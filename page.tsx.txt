"use client"

import { useState } from "react"
import { Button } from "@/components/ui/button"
import { Card, CardContent, CardDescription, CardHeader, CardTitle } from "@/components/ui/card"
import { Input } from "@/components/ui/input"
import { Label } from "@/components/ui/label"
import {
  Heart,
  Shield,
  Users,
  Stethoscope,
  Home,
  CreditCard,
  Brain,
  Mail,
  Phone,
  Menu,
  X,
  Globe,
  Clock,
  TrendingUp,
  Zap,
  UserCheck,
  UserPlus,
  LogIn,
} from "lucide-react"
import Image from "next/image"

export default function BridgebondHealth() {
  const [currentPage, setCurrentPage] = useState("home")
  const [mobileMenuOpen, setMobileMenuOpen] = useState(false)

  const navigation = [
    { id: "home", name: "Home", href: "#" },
    { id: "mission", name: "Our Mission", href: "#" },
    { id: "services", name: "Services", href: "#" },
    { id: "about", name: "About Us", href: "#" },
    { id: "contact", name: "Contact Us", href: "#" },
    { id: "login", name: "Login", href: "#" },
  ]

  const services = [
    {
      icon: Stethoscope,
      title: "Teleconsultations",
      description:
        "Access to verified doctors for real-time virtual consultations with persistent Electronic Health Records (EHRs).",
    },
    {
      icon: Home,
      title: "UK-Style Domiciliary Care",
      description:
        "Trained community carers provide in-home visits with MAR (Medication Administration Records) and wellness reporting.",
    },
    {
      icon: CreditCard,
      title: "Health Credit System",
      description:
        "Secure, traceable health credits that ensure transparency and accountability in healthcare spending.",
    },
    {
      icon: Brain,
      title: "AI Clinical Infrastructure",
      description:
        "Clinical Decision Support (CDS) with drug interaction alerts and pattern recognition for smarter care.",
    },
  ]

  const innovations = [
    {
      icon: Users,
      title: "Dual-Sided Platform",
      description:
        "The only platform designed for both diaspora sponsors and local patients, reflecting real family care structures.",
    },
    {
      icon: Globe,
      title: "Transnational Care Ecosystem",
      description: "Connecting funding, monitoring, clinical governance, and in-person care across continents.",
    },
    {
      icon: Clock,
      title: "Continuity of Care",
      description:
        "Longitudinal care management for chronic conditions with persistent health records and follow-up workflows.",
    },
    {
      icon: Shield,
      title: "Clinical Governance",
      description: "UK-standard care protocols with full traceability and data integration for safety and quality.",
    },
    {
      icon: TrendingUp,
      title: "Learning Health System",
      description: "AI-powered platform that continuously learns from patient interactions to improve outcomes.",
    },
    {
      icon: Zap,
      title: "Multi-Channel Access",
      description: "Web, mobile, WhatsApp, SMS, and voice interfaces for inclusive, low-infrastructure environments.",
    },
  ]

  const stats = [
    { number: "4", label: "Years Experience", description: "Healthcare innovation expertise" },
    { number: "2-Sided", label: "Platform Design", description: "Unique dual-user approach" },
    { number: "UK-Standard", label: "Care Quality", description: "Regulated care protocols" },
    { number: "24/7", label: "Support Available", description: "Round-the-clock assistance" },
  ]

  const brandValues = [
    {
      title: "Accountability",
      description: "We take responsibility for every aspect of care delivery with full transparency and traceability.",
    },
    {
      title: "Empathy",
      description: "Understanding and sharing the feelings of families separated by distance but united by love.",
    },
    {
      title: "Innovation",
      description: "Pioneering new models of cross-border healthcare that bridge gaps with technology.",
    },
    {
      title: "Trust & Transparency",
      description: "Open communication, visible care plans, and reliable service delivery you can count on.",
    },
    {
      title: "Cultural Sensitivity",
      description: "Respecting traditional values while providing modern healthcare solutions.",
    },
    {
      title: "Clinical Excellence",
      description: "UK-standard care protocols ensuring the highest quality of medical service delivery.",
    },
  ]

  const renderPage = () => {
    switch (currentPage) {
      case "home":
        return (
          <div className="space-y-20">
            {/* Hero Section */}
            <section className="relative bg-gradient-to-br from-primary/5 via-background to-secondary/5 py-24 px-4">
              <div className="max-w-7xl mx-auto">
                <div className="text-center mb-16">
                  <div className="mb-8">
                    <h1 className="text-4xl md:text-6xl font-bold text-balance mb-4 text-primary leading-tight">
                      BridgeBond Health
                    </h1>
                    <p className="text-xl md:text-2xl font-semibold text-foreground text-balance leading-relaxed mb-6">
                      Bridging Health Gaps with Trust, One Family at a Time
                    </p>
                  </div>
                  <p className="text-lg md:text-xl text-muted-foreground text-balance mb-10 leading-relaxed max-w-4xl mx-auto">
                    The world's first cross-border digital health platform designed for diaspora families. We transform
                    informal healthcare arrangements into formal, accountable, and transparent care systems.
                  </p>
                  <div className="flex flex-col sm:flex-row gap-4 justify-center mb-16">
                    <Button
                      size="lg"
                      className="bg-primary hover:bg-primary/90 text-primary-foreground text-lg px-8 py-4"
                    >
                      Get Started Today
                    </Button>
                    <Button
                      variant="outline"
                      size="lg"
                      className="text-lg px-8 py-4 border-primary text-primary hover:bg-primary/5 bg-transparent"
                    >
                      Watch Demo
                    </Button>
                  </div>
                </div>

                <div className="mb-16">
                  <div className="max-w-4xl mx-auto">
                    <div className="bg-gradient-to-br from-primary/10 to-secondary/10 rounded-3xl p-8 backdrop-blur-sm">
                      <img
                        src="/african-doctor-conducting-telemedicine-consultatio.jpg"
                        alt="Telemedicine consultation"
                        className="w-full h-64 md:h-80 object-cover rounded-2xl shadow-2xl"
                      />
                    </div>
                  </div>
                </div>

                <div className="max-w-4xl mx-auto">
                  <div className="grid md:grid-cols-2 gap-6">
                    <Card className="bg-white/80 backdrop-blur-sm shadow-lg hover:shadow-xl transition-all duration-300 cursor-pointer hover:-translate-y-1">
                      <CardContent className="p-8 text-center">
                        <div className="w-16 h-16 bg-primary/10 rounded-full flex items-center justify-center mx-auto mb-4">
                          <Users className="w-8 h-8 text-primary" />
                        </div>
                        <h3 className="text-xl font-semibold text-foreground mb-2">Diaspora Sponsor</h3>
                        <p className="text-muted-foreground">Monitor & fund care from anywhere in the world</p>
                      </CardContent>
                    </Card>
                    <Card className="bg-white/80 backdrop-blur-sm shadow-lg hover:shadow-xl transition-all duration-300 cursor-pointer hover:-translate-y-1">
                      <CardContent className="p-8 text-center">
                        <div className="w-16 h-16 bg-secondary/10 rounded-full flex items-center justify-center mx-auto mb-4">
                          <Heart className="w-8 h-8 text-secondary" />
                        </div>
                        <h3 className="text-xl font-semibold text-foreground mb-2">Local Patient</h3>
                        <p className="text-muted-foreground">Receive quality healthcare at home in Nigeria</p>
                      </CardContent>
                    </Card>
                  </div>
                </div>
              </div>
            </section>

            {/* Stats Section */}
            <section className="py-16 px-4 bg-muted/30">
              <div className="max-w-6xl mx-auto">
                <div className="grid md:grid-cols-4 gap-8">
                  {stats.map((stat, index) => (
                    <div key={index} className="text-center">
                      <div className="text-4xl md:text-5xl font-bold text-primary mb-2">{stat.number}</div>
                      <div className="text-lg font-semibold text-foreground mb-1">{stat.label}</div>
                      <div className="text-sm text-muted-foreground">{stat.description}</div>
                    </div>
                  ))}
                </div>
              </div>
            </section>

            {/* Innovation Section */}
            <section className="py-20 px-4">
              <div className="max-w-7xl mx-auto">
                <div className="text-center mb-16">
                  <h2 className="text-4xl md:text-5xl font-bold mb-6 text-foreground">
                    Our <span className="text-primary">Innovation</span>
                  </h2>
                  <p className="text-xl text-muted-foreground max-w-4xl mx-auto text-balance">
                    BridgeBond Health reimagines how diaspora families engage with healthcare systems, creating a new
                    class of digital health infrastructure that connects continents.
                  </p>
                </div>
                <div className="grid md:grid-cols-2 lg:grid-cols-3 gap-8">
                  {innovations.map((innovation, index) => (
                    <Card
                      key={index}
                      className="border-border bg-card hover:shadow-xl transition-all duration-300 hover:-translate-y-1"
                    >
                      <CardHeader>
                        <div className="w-16 h-16 bg-primary/10 rounded-2xl flex items-center justify-center mb-4">
                          <innovation.icon className="w-8 h-8 text-primary" />
                        </div>
                        <CardTitle className="text-xl text-card-foreground">{innovation.title}</CardTitle>
                      </CardHeader>
                      <CardContent>
                        <CardDescription className="text-muted-foreground text-base leading-relaxed">
                          {innovation.description}
                        </CardDescription>
                      </CardContent>
                    </Card>
                  ))}
                </div>
              </div>
            </section>

            {/* Services Section */}
            <section className="py-20 px-4 bg-gradient-to-br from-primary/5 to-secondary/5">
              <div className="max-w-7xl mx-auto">
                <div className="text-center mb-16">
                  <h2 className="text-4xl md:text-5xl font-bold mb-6 text-foreground">
                    Comprehensive <span className="text-secondary">Care Services</span>
                  </h2>
                  <p className="text-xl text-muted-foreground max-w-3xl mx-auto text-balance">
                    From AI-powered clinical tools to UK-standard domiciliary care, we provide integrated healthcare
                    solutions that bridge continents.
                  </p>
                </div>
                <div className="grid md:grid-cols-2 gap-8">
                  {services.map((service, index) => (
                    <Card
                      key={index}
                      className="border-border bg-card/80 backdrop-blur-sm hover:shadow-xl transition-all duration-300"
                    >
                      <CardHeader>
                        <div className="flex items-center space-x-4">
                          <div className="w-16 h-16 bg-gradient-to-br from-primary/10 to-secondary/10 rounded-2xl flex items-center justify-center">
                            <service.icon className="w-8 h-8 text-primary" />
                          </div>
                          <CardTitle className="text-2xl text-card-foreground">{service.title}</CardTitle>
                        </div>
                      </CardHeader>
                      <CardContent>
                        <CardDescription className="text-muted-foreground text-lg leading-relaxed">
                          {service.description}
                        </CardDescription>
                      </CardContent>
                    </Card>
                  ))}
                </div>
              </div>
            </section>

            <section className="py-20 px-4">
              <div className="max-w-7xl mx-auto">
                <div className="text-center mb-16">
                  <h2 className="text-4xl md:text-5xl font-bold mb-6 text-foreground">
                    Connecting <span className="text-primary">UK</span> to{" "}
                    <span className="text-secondary">Nigeria</span>
                  </h2>
                  <p className="text-xl text-muted-foreground max-w-3xl mx-auto text-balance">
                    Experience seamless healthcare delivery across continents with our advanced telemedicine platform.
                  </p>
                </div>
                <div className="space-y-8">
                  <div className="max-w-4xl mx-auto">
                    <img
                      src="/uk-doctor-consulting-with-nigerian-patient-via-vid.jpg"
                      alt="UK to Nigeria telemedicine"
                      className="w-full h-64 md:h-80 object-cover rounded-3xl shadow-2xl"
                    />
                  </div>
                  <div className="max-w-4xl mx-auto">
                    <img
                      src="/african-family-receiving-healthcare-consultation-a.jpg"
                      alt="African family healthcare"
                      className="w-full h-64 md:h-80 object-cover rounded-3xl shadow-2xl"
                    />
                  </div>
                </div>
              </div>
            </section>

            {/* CTA Section */}
            <section className="py-20 px-4">
              <div className="max-w-4xl mx-auto text-center">
                <div className="bg-gradient-to-br from-primary to-secondary rounded-3xl p-12 text-white">
                  <h2 className="text-3xl md:text-4xl font-bold mb-6">
                    Ready to Transform Healthcare for Your Family?
                  </h2>
                  <p className="text-xl mb-8 opacity-90">
                    Join the revolution in cross-border healthcare. Experience peace of mind with transparent,
                    accountable, and professional care coordination.
                  </p>
                  <div className="flex flex-col sm:flex-row gap-4 justify-center">
                    <Button size="lg" variant="secondary" className="text-lg px-8 py-4">
                      Start Your Journey
                    </Button>
                    <Button
                      size="lg"
                      variant="outline"
                      className="text-lg px-8 py-4 border-white text-white hover:bg-white/10 bg-transparent"
                    >
                      Schedule Consultation
                    </Button>
                  </div>
                </div>
              </div>
            </section>
          </div>
        )

      case "login":
        return (
          <div className="py-16 px-4">
            <div className="max-w-4xl mx-auto">
              <div className="text-center mb-12">
                <h1 className="text-4xl md:text-5xl font-bold mb-6 text-foreground">Choose Your Login</h1>
                <p className="text-xl text-muted-foreground">
                  Access your BridgeBond Health account based on your role
                </p>
              </div>

              <div className="grid md:grid-cols-3 gap-8">
                {/* Patient Login */}
                <Card className="border-border bg-card hover:shadow-xl transition-all duration-300 hover:-translate-y-1">
                  <CardHeader className="text-center">
                    <div className="w-20 h-20 bg-primary/10 rounded-full flex items-center justify-center mx-auto mb-4">
                      <Heart className="w-10 h-10 text-primary" />
                    </div>
                    <CardTitle className="text-2xl text-primary">Patient Login</CardTitle>
                    <CardDescription>Access your health records and care plans</CardDescription>
                  </CardHeader>
                  <CardContent className="space-y-4">
                    <div>
                      <Label htmlFor="patient-email">Email</Label>
                      <Input id="patient-email" type="email" placeholder="patient@example.com" />
                    </div>
                    <div>
                      <Label htmlFor="patient-password">Password</Label>
                      <Input id="patient-password" type="password" placeholder="••••••••" />
                    </div>
                    <Button className="w-full bg-primary hover:bg-primary/90">
                      <LogIn className="w-4 h-4 mr-2" />
                      Login as Patient
                    </Button>
                    <div className="text-center">
                      <Button variant="link" className="text-sm text-primary">
                        Forgot password?
                      </Button>
                    </div>
                  </CardContent>
                </Card>

                {/* Doctor Login */}
                <Card className="border-border bg-card hover:shadow-xl transition-all duration-300 hover:-translate-y-1">
                  <CardHeader className="text-center">
                    <div className="w-20 h-20 bg-secondary/10 rounded-full flex items-center justify-center mx-auto mb-4">
                      <Stethoscope className="w-10 h-10 text-secondary" />
                    </div>
                    <CardTitle className="text-2xl text-secondary">Doctor Login</CardTitle>
                    <CardDescription>Access patient records and consultation tools</CardDescription>
                  </CardHeader>
                  <CardContent className="space-y-4">
                    <div>
                      <Label htmlFor="doctor-email">Email</Label>
                      <Input id="doctor-email" type="email" placeholder="doctor@example.com" />
                    </div>
                    <div>
                      <Label htmlFor="doctor-password">Password</Label>
                      <Input id="doctor-password" type="password" placeholder="••••••••" />
                    </div>
                    <Button className="w-full bg-secondary hover:bg-secondary/90">
                      <UserCheck className="w-4 h-4 mr-2" />
                      Login as Doctor
                    </Button>
                    <div className="text-center">
                      <Button variant="link" className="text-sm text-secondary">
                        Forgot password?
                      </Button>
                    </div>
                  </CardContent>
                </Card>

                {/* Sponsor Login */}
                <Card className="border-border bg-card hover:shadow-xl transition-all duration-300 hover:-translate-y-1">
                  <CardHeader className="text-center">
                    <div className="w-20 h-20 bg-accent/10 rounded-full flex items-center justify-center mx-auto mb-4">
                      <Users className="w-10 h-10 text-accent" />
                    </div>
                    <CardTitle className="text-2xl text-accent">Sponsor Login</CardTitle>
                    <CardDescription>Monitor and fund care for your loved ones</CardDescription>
                  </CardHeader>
                  <CardContent className="space-y-4">
                    <div>
                      <Label htmlFor="sponsor-email">Email</Label>
                      <Input id="sponsor-email" type="email" placeholder="sponsor@example.com" />
                    </div>
                    <div>
                      <Label htmlFor="sponsor-password">Password</Label>
                      <Input id="sponsor-password" type="password" placeholder="••••••••" />
                    </div>
                    <Button className="w-full bg-accent hover:bg-accent/90">
                      <UserPlus className="w-4 h-4 mr-2" />
                      Login as Sponsor
                    </Button>
                    <div className="text-center">
                      <Button variant="link" className="text-sm text-accent">
                        Forgot password?
                      </Button>
                    </div>
                  </CardContent>
                </Card>
              </div>

              <div className="text-center mt-12">
                <p className="text-muted-foreground mb-4">Don't have an account?</p>
                <Button variant="outline" size="lg" className="text-lg px-8 py-4 bg-transparent">
                  Sign Up Today
                </Button>
              </div>
            </div>
          </div>
        )

      case "mission":
        return (
          <div className="space-y-16 py-16 px-4">
            <div className="max-w-4xl mx-auto">
              <h1 className="text-4xl md:text-5xl font-bold text-center mb-16 text-foreground">Our Vision & Mission</h1>

              <div className="space-y-12">
                <Card className="border-border bg-card">
                  <CardHeader>
                    <CardTitle className="text-2xl text-primary">Vision Statement</CardTitle>
                  </CardHeader>
                  <CardContent>
                    <p className="text-lg text-card-foreground leading-relaxed">
                      To become the world's leading cross-border digital health platform, empowering diaspora
                      communities to provide seamless, high-quality healthcare for their loved ones across continents,
                      while setting new standards for transparency, accountability, and compassionate care delivery.
                    </p>
                  </CardContent>
                </Card>

                <Card className="border-border bg-card">
                  <CardHeader>
                    <CardTitle className="text-2xl text-secondary">Mission Statement</CardTitle>
                  </CardHeader>
                  <CardContent>
                    <p className="text-lg text-card-foreground leading-relaxed">
                      We are building a dual-sided digital health platform that bridges the healthcare gap between
                      diaspora families and their loved ones in Nigeria. Through innovative technology, verified
                      healthcare professionals, and transparent care coordination, we transform informal, high-risk
                      healthcare arrangements into formal, accountable, and effective care systems that provide peace of
                      mind for families separated by distance.
                    </p>
                  </CardContent>
                </Card>
              </div>
            </div>
          </div>
        )

      case "services":
        return (
          <div className="space-y-16 py-16 px-4">
            <div className="max-w-6xl mx-auto">
              <h1 className="text-4xl md:text-5xl font-bold text-center mb-8 text-foreground">Our Core Services</h1>
              <p className="text-xl text-center text-muted-foreground mb-16 max-w-3xl mx-auto">
                We provide peace of mind through a suite of integrated healthcare solutions.
              </p>

              <div className="grid md:grid-cols-2 gap-8">
                {services.map((service, index) => (
                  <Card key={index} className="border-border bg-card hover:shadow-lg transition-shadow">
                    <CardHeader>
                      <div className="flex items-center space-x-4">
                        <div className="w-12 h-12 bg-primary/10 rounded-lg flex items-center justify-center">
                          <service.icon className="w-6 h-6 text-primary" />
                        </div>
                        <CardTitle className="text-xl text-card-foreground">{service.title}</CardTitle>
                      </div>
                    </CardHeader>
                    <CardContent>
                      <CardDescription className="text-muted-foreground text-base">
                        {service.description}
                      </CardDescription>
                    </CardContent>
                  </Card>
                ))}
              </div>
            </div>
          </div>
        )

      case "about":
        return (
          <div className="space-y-16 py-16 px-4">
            <div className="max-w-6xl mx-auto">
              <h1 className="text-4xl md:text-5xl font-bold text-center mb-16 text-foreground">Meet the Founder</h1>

              <Card className="border-border bg-card mb-16">
                <CardContent className="p-8">
                  <div className="grid md:grid-cols-3 gap-8 items-center">
                    <div className="md:col-span-1">
                      <div className="w-48 h-48 bg-muted rounded-full mx-auto flex items-center justify-center">
                        <span className="text-4xl font-bold text-muted-foreground">EO</span>
                      </div>
                    </div>
                    <div className="md:col-span-2">
                      <h3 className="text-2xl font-bold mb-4 text-card-foreground">Eleanor Ojo-Emovon</h3>
                      <p className="text-lg text-muted-foreground leading-relaxed">
                        With over 4 years of experience in healthcare innovation and cross-border care coordination,
                        Eleanor brings deep personal insight into the challenges faced by diaspora families. Her vision
                        for Bridgebond Health stems from witnessing firsthand the gaps in healthcare access and the need
                        for transparent, accountable care systems that bridge geographical divides.
                      </p>
                    </div>
                  </div>
                </CardContent>
              </Card>

              <div>
                <h2 className="text-3xl font-bold text-center mb-12 text-foreground">Our Brand Values</h2>
                <div className="grid md:grid-cols-2 lg:grid-cols-3 gap-6">
                  {brandValues.map((value, index) => (
                    <Card key={index} className="border-border bg-card">
                      <CardHeader>
                        <CardTitle className="text-lg text-primary">{value.title}</CardTitle>
                      </CardHeader>
                      <CardContent>
                        <CardDescription className="text-muted-foreground">{value.description}</CardDescription>
                      </CardContent>
                    </Card>
                  ))}
                </div>
              </div>
            </div>
          </div>
        )

      case "contact":
        return (
          <div className="space-y-16 py-16 px-4">
            <div className="max-w-4xl mx-auto text-center">
              <h1 className="text-4xl md:text-5xl font-bold mb-8 text-foreground">Ready to Bridge the Gap?</h1>
              <p className="text-xl text-muted-foreground mb-16">
                Get in touch with us to learn more about how we can help your family.
              </p>

              <div className="grid md:grid-cols-2 gap-8 max-w-2xl mx-auto">
                <Card className="border-border bg-card">
                  <CardContent className="p-8 text-center">
                    <div className="w-16 h-16 bg-primary/10 rounded-full flex items-center justify-center mx-auto mb-4">
                      <Mail className="w-8 h-8 text-primary" />
                    </div>
                    <h3 className="text-xl font-semibold mb-2 text-card-foreground">Email Us</h3>
                    <p className="text-muted-foreground">contact@bridgebondhealth.com</p>
                  </CardContent>
                </Card>

                <Card className="border-border bg-card">
                  <CardContent className="p-8 text-center">
                    <div className="w-16 h-16 bg-secondary/10 rounded-full flex items-center justify-center mx-auto mb-4">
                      <Phone className="w-8 h-8 text-secondary" />
                    </div>
                    <h3 className="text-xl font-semibold mb-2 text-card-foreground">Call Us</h3>
                    <p className="text-muted-foreground">+44 (0) 20 1234 5678</p>
                  </CardContent>
                </Card>
              </div>

              <div className="mt-12">
                <Button size="lg" className="bg-primary hover:bg-primary/90 text-primary-foreground">
                  Schedule a Consultation
                </Button>
              </div>
            </div>
          </div>
        )

      default:
        return null
    }
  }

  return (
    <div className="min-h-screen bg-background">
      {/* Navigation */}
      <nav className="bg-background/95 backdrop-blur-sm border-b border-border sticky top-0 z-50">
        <div className="max-w-7xl mx-auto px-4">
          <div className="flex justify-between items-center h-20">
            <div className="flex items-center space-x-3">
              <Image src="/logo.png" alt="Bridgebond Health Logo" width={220} height={80} className="h-16 w-auto" />
            </div>

            {/* Desktop Navigation */}
            <div className="hidden md:flex space-x-8">
              {navigation.map((item) => (
                <button
                  key={item.id}
                  onClick={() => setCurrentPage(item.id)}
                  className={`px-4 py-2 text-sm font-medium transition-colors rounded-lg ${
                    currentPage === item.id
                      ? "text-primary bg-primary/10"
                      : "text-muted-foreground hover:text-foreground hover:bg-muted"
                  }`}
                >
                  {item.name}
                </button>
              ))}
            </div>

            {/* Mobile menu button */}
            <div className="md:hidden">
              <button
                onClick={() => setMobileMenuOpen(!mobileMenuOpen)}
                className="text-muted-foreground hover:text-foreground p-2"
              >
                {mobileMenuOpen ? <X className="w-6 h-6" /> : <Menu className="w-6 h-6" />}
              </button>
            </div>
          </div>

          {/* Mobile Navigation */}
          {mobileMenuOpen && (
            <div className="md:hidden border-t border-border">
              <div className="py-2 space-y-1">
                {navigation.map((item) => (
                  <button
                    key={item.id}
                    onClick={() => {
                      setCurrentPage(item.id)
                      setMobileMenuOpen(false)
                    }}
                    className={`block w-full text-left px-3 py-2 text-sm font-medium transition-colors rounded-lg ${
                      currentPage === item.id
                        ? "text-primary bg-primary/10"
                        : "text-muted-foreground hover:text-foreground hover:bg-muted"
                    }`}
                  >
                    {item.name}
                  </button>
                ))}
              </div>
            </div>
          )}
        </div>
      </nav>

      {/* Main Content */}
      <main>{renderPage()}</main>

      {/* Footer */}
      <footer className="bg-muted/50 border-t border-border py-16 px-4">
        <div className="max-w-7xl mx-auto">
          <div className="grid md:grid-cols-4 gap-8">
            <div className="md:col-span-2">
              <div className="flex items-center space-x-3 mb-6">
                <Image src="/logo.png" alt="Bridgebond Health Logo" width={180} height={60} className="h-12 w-auto" />
              </div>
              <p className="text-muted-foreground mb-4 text-lg">
                Bridging health gaps with trust, one family at a time. The world's first cross-border digital health
                platform for diaspora families.
              </p>
            </div>

            <div>
              <h4 className="font-semibold text-foreground mb-4">Quick Links</h4>
              <div className="space-y-2">
                {navigation.map((item) => (
                  <button
                    key={item.id}
                    onClick={() => setCurrentPage(item.id)}
                    className="block text-muted-foreground hover:text-primary transition-colors"
                  >
                    {item.name}
                  </button>
                ))}
              </div>
            </div>

            <div>
              <h4 className="font-semibold text-foreground mb-4">Contact</h4>
              <div className="space-y-2 text-muted-foreground">
                <p>contact@bridgebondhealth.com</p>
                <p>+44 (0) 20 1234 5678</p>
              </div>
            </div>
          </div>

          <div className="border-t border-border mt-12 pt-8 text-center text-muted-foreground">
            <p>&copy; 2024 Bridgebond Health. All rights reserved.</p>
          </div>
        </div>
      </footer>
    </div>
  )
}
