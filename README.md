# https://corekits.framer.website/
# https://rsms.me/inter/
# https://weareyellowball.com/
# https://www.kitsapexterior.com/

## --preset b1aKNFeoD


// app/layout.tsx

import { Inter } from "next/font/google";

const inter = Inter({
  subsets: ["latin"],
  variable: "--font-inter",
});

export default function RootLayout({
  children,
}: {
  children: React.ReactNode;
}) {
  return (
    <html lang="en" className={inter.variable}>
      <body>{children}</body>
    </html>
  );
}

body {
  font-family: var(--font-inter), system-ui, sans-serif;
}



html {
  font-family: var(--font-inter), Inter, sans-serif;

  font-optical-sizing: auto;
  font-feature-settings: "liga" 1, "calt" 1;

  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;

  text-rendering: optimizeLegibility;
}
