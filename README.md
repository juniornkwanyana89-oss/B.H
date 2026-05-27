# B.H// DEPLOYMENT READY NEXT.JS + TAILWIND PROJECT
// ==========================================
//
// 1. Create a new Next.js app:
// npx create-next-app@latest branded-heights
//
// 2. Install Tailwind:
// npm install -D tailwindcss postcss autoprefixer
// npx tailwindcss init -p
//
// 3. Replace app/page.js with the code below.
//
// 4. Replace app/globals.css with:
//
// @tailwind base;
// @tailwind components;
// @tailwind utilities;
//
// body {
//   background: #0a0a0a;
// }
//
// 5. Run locally:
// npm run dev
//
// 6. Push to GitHub and deploy on Vercel.
// ==========================================

export default function BrandedHeightsWebsite() {
  return (
    <div className="min-h-screen bg-neutral-950 text-white font-sans">
      {/* Hero Section */}
      <section className="relative overflow-hidden border-b border-neutral-800">
        <div className="absolute inset-0 bg-gradient-to-br from-orange-500/20 via-transparent to-neutral-950"></div>
        <div className="relative max-w-7xl mx-auto px-6 py-24 lg:py-32">
          <div className="grid lg:grid-cols-2 gap-14 items-center">
            <div>
              <div className="inline-flex items-center rounded-full border border-orange-500/30 bg-orange-500/10 px-4 py-2 text-sm text-orange-300 mb-6">
                BRANDED HEIGHTS
              </div>

              <h1 className="text-5xl md:text-7xl font-black leading-tight tracking-tight">
                Elevate Your
                <span className="block text-orange-400">Brand Presence</span>
              </h1>

              <p className="mt-6 text-lg text-neutral-300 max-w-xl leading-relaxed">
                Branded Heights helps businesses stand out with premium branding,
                digital growth strategies, professional visuals, and modern online experiences.
              </p>

              <div className="mt-10 flex flex-wrap gap-4">
                <button className="px-7 py-4 rounded-2xl bg-orange-500 hover:bg-orange-400 transition font-semibold text-black shadow-2xl shadow-orange-500/30">
                  Get Started
                </button>

                <button className="px-7 py-4 rounded-2xl border border-neutral-700 hover:border-orange-400 hover:text-orange-300 transition">
                  View Services
                </button>
              </div>
            </div>

            <div className="relative">
              <div className="absolute inset-0 bg-orange-500/20 blur-3xl rounded-full"></div>
              <div className="relative bg-neutral-900 border border-neutral-800 rounded-[2rem] p-8 shadow-2xl">
                <div className="space-y-6">
                  <div className="flex items-center justify-between">
                    <div>
                      <p className="text-sm text-neutral-400">Brand Growth</p>
                      <h3 className="text-3xl font-bold">+240%</h3>
                    </div>
                    <div className="h-14 w-14 rounded-2xl bg-orange-500 flex items-center justify-center text-black font-black text-xl">
                      BH
                    </div>
                  </div>

                  <div className="grid grid-cols-2 gap-4">
                    <div className="rounded-2xl bg-neutral-800 p-5">
                      <p className="text-sm text-neutral-400">Projects</p>
                      <h4 className="text-2xl font-bold mt-2">120+</h4>
                    </div>

                    <div className="rounded-2xl bg-neutral-800 p-5">
                      <p className="text-sm text-neutral-400">Clients</p>
                      <h4 className="text-2xl font-bold mt-2">85+</h4>
                    </div>
                  </div>

                  <div className="rounded-2xl bg-gradient-to-r from-orange-500 to-orange-300 text-black p-6">
                    <h4 className="text-2xl font-black">Professional. Modern. Scalable.</h4>
                    <p className="mt-2 font-medium">
                      We help businesses create a premium digital image that attracts more customers.
                    </p>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </section>

      {/* Services */}
      <section className="max-w-7xl mx-auto px-6 py-24">
        <div className="text-center mb-16">
          <p className="text-orange-400 font-semibold uppercase tracking-widest">Our Services</p>
          <h2 className="text-4xl md:text-5xl font-black mt-4">What We Do</h2>
        </div>

        <div className="grid md:grid-cols-2 lg:grid-cols-4 gap-6">
          {[
            {
              title: 'Brand Strategy',
              desc: 'Build a strong and recognizable business identity.'
            },
            {
              title: 'Social Media Growth',
              desc: 'Create engaging content and increase online visibility.'
            },
            {
              title: 'Website Design',
              desc: 'Modern responsive websites built for conversions.'
            },
            {
              title: 'Photo & Visual Editing',
              desc: 'Professional visuals that elevate your business image.'
            }
          ].map((service, index) => (
            <div
              key={index}
              className="bg-neutral-900 border border-neutral-800 rounded-3xl p-7 hover:border-orange-500/50 transition duration-300 hover:-translate-y-1"
            >
              <div className="h-14 w-14 rounded-2xl bg-orange-500/10 border border-orange-500/20 flex items-center justify-center text-orange-400 font-bold text-xl">
                0{index + 1}
              </div>

              <h3 className="text-2xl font-bold mt-6">{service.title}</h3>
              <p className="mt-4 text-neutral-400 leading-relaxed">{service.desc}</p>
            </div>
          ))}
        </div>
      </section>

      {/* Why Choose Us */}
      <section className="bg-neutral-900 border-y border-neutral-800">
        <div className="max-w-7xl mx-auto px-6 py-24 grid lg:grid-cols-2 gap-16 items-center">
          <div>
            <p className="text-orange-400 font-semibold uppercase tracking-widest">
              Why Branded Heights
            </p>

            <h2 className="text-4xl md:text-5xl font-black mt-4 leading-tight">
              Helping Businesses Reach New Heights
            </h2>

            <p className="mt-6 text-neutral-300 text-lg leading-relaxed">
              We combine modern branding, digital marketing, and visual design to help businesses create authority and attract customers online.
            </p>
          </div>

          <div className="space-y-5">
            {[
              'Modern and aesthetic branding',
              'Fast and responsive websites',
              'Professional visual editing',
              'Growth-focused strategies',
            ].map((item, index) => (
              <div
                key={index}
                className="flex items-center gap-4 bg-neutral-950 border border-neutral-800 rounded-2xl p-5"
              >
                <div className="h-10 w-10 rounded-full bg-orange-500 text-black font-black flex items-center justify-center">
                  ✓
                </div>
                <p className="text-lg">{item}</p>
              </div>
            ))}
          </div>
        </div>
      </section>

      {/* Contact Section */}
      <section className="max-w-6xl mx-auto px-6 py-24">
        <div className="grid lg:grid-cols-2 gap-10">
          <div className="bg-neutral-900 border border-neutral-800 rounded-[2rem] p-10">
            <p className="text-orange-400 font-semibold uppercase tracking-widest">
              Contact Us
            </p>

            <h2 className="text-4xl font-black mt-4 leading-tight">
              Let’s Build Your Brand
            </h2>

            <p className="mt-6 text-neutral-300 leading-relaxed text-lg">
              Ready to elevate your business? Reach out to Branded Heights for branding, websites, digital growth, and professional visuals.
            </p>
          </div>

          <div className="bg-neutral-900 border border-neutral-800 rounded-[2rem] p-10 space-y-8">
            <div>
              <p className="text-sm uppercase tracking-widest text-orange-400">Phone & WhatsApp</p>
              <a
                href="https://wa.me/27768793116"
                className="text-2xl font-bold hover:text-orange-400 transition"
              >
                076 879 3116
              </a>
            </div>

            <div>
              <p className="text-sm uppercase tracking-widest text-orange-400">Email</p>
              <a
                href="mailto:Branded.Heights@gmail.com"
                className="text-2xl font-bold break-all hover:text-orange-400 transition"
              >
                Branded.Heights@gmail.com
              </a>
            </div>

            <div>
              <p className="text-sm uppercase tracking-widest text-orange-400">Business Name</p>
              <h3 className="text-2xl font-bold">Branded Heights</h3>
            </div>
          </div>
        </div>
      </section>

      {/* CTA */}
      <section className="max-w-5xl mx-auto px-6 pb-24">
        <div className="rounded-[2rem] border border-orange-500/20 bg-gradient-to-r from-orange-500/20 to-neutral-900 p-10 md:p-16 text-center">
          <h2 className="text-4xl md:text-5xl font-black leading-tight">
            Ready To Grow Your Business?
          </h2>

          <p className="mt-6 text-neutral-300 text-lg max-w-2xl mx-auto">
            Partner with Branded Heights and create a professional online presence that drives attention, trust, and sales.
          </p>

          <a
            href="https://wa.me/27768793116"
            className="inline-block mt-10 px-8 py-4 rounded-2xl bg-orange-500 hover:bg-orange-400 transition text-black font-bold text-lg shadow-xl shadow-orange-500/20"
          >
            Contact Us On WhatsApp
          </a>
        </div>
      </section>

      {/* Footer */}
      <footer className="border-t border-neutral-800">
        <div className="max-w-7xl mx-auto px-6 py-10 flex flex-col md:flex-row items-center justify-between gap-6">
          <div>
            <h3 className="text-2xl font-black text-orange-400">Branded Heights</h3>
            <p className="text-neutral-400 mt-2">
              Elevating brands through modern digital experiences.
            </p>
          </div>

          <div className="text-neutral-500 text-sm text-center md:text-right">
            <p>076 879 3116</p>
            <p>Branded.Heights@gmail.com</p>
            <p className="mt-2">© 2026 Branded Heights. All rights reserved.</p>
          </div>
        </div>
      </footer>
    </div>
  )
}
