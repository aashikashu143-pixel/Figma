# Ex08 Event Registration Web Application
## Date:28-12-2025

## AIM:
To design, develop and deploy a web application for event registration using Figma UI tool.

## UI DESIGN TOOL:
Figma

## DESIGN STEPS:

### Step 1:
Use frames to represent screens or sections.

### Step 2:
Add column grids for consistent spacing and alignment.

### Step 3:
Insert shapes, text, buttons, and icons.

### Step 4:
Use Auto Layout for flexible, responsive design.

### Step 5:
Define color, text, and effect styles globally for consistency.

### Step 6:
Name layers logically and group related elements.

### Step 6:
Link frames to show navigation or interactions.

### Step 7:
Select the specific frame while generating code using Anima plugin.

## CODE:
```
page1
html
import React from "react";
import rectangle1 from "./rectangle-1.png";
import rectangle2 from "./rectangle-2.png";
import rectangle7 from "./rectangle-7.png";

export const IphoneProMax = () => {
  return (
    <div className="bg-white w-full min-w-[562px] min-h-[956px] relative">
      <img
        className="absolute top-0 left-0 w-[562px] h-[92px] object-cover"
        alt="Rectangle"
        src={rectangle1}
      />

      <img
        className="absolute top-[117px] left-[122px] w-[278px] h-56 object-cover"
        alt="Rectangle"
        src={rectangle2}
      />

      <div className="absolute top-[366px] left-14 w-[480px] h-[81px] bg-[#ff0000]" />

      <div className="absolute top-[375px] left-[83px] [font-family:'Jomhuria-Regular',Helvetica] font-normal text-white text-[85px] tracking-[0] leading-[normal] whitespace-nowrap">
        CELENZA DAY EVENTS
      </div>

      <div className="absolute top-[375px] left-[83px] [font-family:'Jomhuria-Regular',Helvetica] font-normal text-white text-[85px] tracking-[0] leading-[normal] whitespace-nowrap">
        CELENZA DAY EVENTS
      </div>

      <div className="absolute top-[467px] left-[178px] w-[193px] h-14 bg-[#50ff00]" />

      <div className="absolute top-[467px] left-[211px] [font-family:'Kodchasan-Regular',Helvetica] font-normal text-black text-[40px] tracking-[0] leading-[normal]">
        LOGIN
      </div>

      <div className="absolute top-[530px] left-[178px] w-[193px] h-[59px] bg-[#10ff00]" />

      <div className="absolute top-[530px] left-[191px] [font-family:'Kreon-Regular',Helvetica] font-normal text-black text-[40px] tracking-[0] leading-[normal]">
        REGISTER
      </div>

      <img
        className="absolute top-[601px] left-0 w-[562px] h-[355px] object-cover"
        alt="Rectangle"
        src={rectangle7}
      />
    </div>
  );
};
css
@tailwind components;
@tailwind utilities;

@layer components {
  .all-\[unset\] {
    all: unset;
  }
}

:root {
  --animate-spin: spin 1s linear infinite;
}

.animate-fade-in {
  animation: fade-in 1s var(--animation-delay, 0s) ease forwards;
}

.animate-fade-up {
  animation: fade-up 1s var(--animation-delay, 0s) ease forwards;
}

.animate-marquee {
  animation: marquee var(--duration) infinite linear;
}

.animate-marquee-vertical {
  animation: marquee-vertical var(--duration) linear infinite;
}

.animate-shimmer {
  animation: shimmer 8s infinite;
}

.animate-spin {
  animation: var(--animate-spin);
}

@keyframes spin {
  to {
    transform: rotate(1turn);
  }
}

@keyframes image-glow {
  0% {
    opacity: 0;
    animation-timing-function: cubic-bezier(0.74, 0.25, 0.76, 1);
  }

  10% {
    opacity: 0.7;
    animation-timing-function: cubic-bezier(0.12, 0.01, 0.08, 0.99);
  }

  to {
    opacity: 0.4;
  }
}

@keyframes fade-in {
  0% {
    opacity: 0;
    transform: translateY(-10px);
  }

  to {
    opacity: 1;
    transform: none;
  }
}

@keyframes fade-up {
  0% {
    opacity: 0;
    transform: translateY(20px);
  }

  to {
    opacity: 1;
    transform: none;
  }
}

@keyframes shimmer {
  0%,
  90%,
  to {
    background-position: calc(-100% - var(--shimmer-width)) 0;
  }

  30%,
  60% {
    background-position: calc(100% + var(--shimmer-width)) 0;
  }
}

@keyframes marquee {
  0% {
    transform: translate(0);
  }

  to {
    transform: translateX(calc(-100% - var(--gap)));
  }
}

@keyframes marquee-vertical {
  0% {
    transform: translateY(0);
  }

  to {
    transform: translateY(calc(-100% - var(--gap)));
  }
}
js
/** @type {import('tailwindcss').Config} */
module.exports = {
  content: ["./src/**/*.{html,js,ts,jsx,tsx}"],
  theme: {
    extend: {},
  },
  plugins: [],
};
page2
jsx
import React from "react";

export const IphoneProMax = () => {
  return (
    <div className="bg-white w-full min-w-[589px] min-h-[956px] relative">
      <div className="absolute top-[19px] left-[19px] w-[545px] h-[83px] bg-[#d9d9d9]" />

      <div className="absolute top-[19px] left-[54px] [font-family:'Jomhuria-Regular',Helvetica] font-normal text-white text-[95px] tracking-[0] leading-[normal] whitespace-nowrap">
        CELENZA DAY EVENTS
      </div>

      <div className="absolute top-[375px] left-[83px] [font-family:'Jomhuria-Regular',Helvetica] font-normal text-white text-[85px] tracking-[0] leading-[normal] whitespace-nowrap">
        CEPRLENZA DAY EVENTS
      </div>

      <div className="absolute top-96 left-[115px] [font-family:'Jomhuria-Regular',Helvetica] font-normal text-black text-[85px] tracking-[0] leading-[normal] whitespace-nowrap">
        PRIZ DISTRIBUTION
      </div>

      <div className="absolute top-28 left-[115px] [font-family:'Jomhuria-Regular',Helvetica] font-normal text-black text-[95px] tracking-[0] leading-[normal] whitespace-nowrap">
        WELCOME WHISHES
      </div>

      <div className="absolute top-[175px] left-[115px] [font-family:'Jomhuria-Regular',Helvetica] font-normal text-black text-[95px] tracking-[0] leading-[normal]">
        AUTO EXPO
      </div>

      <div className="absolute top-[244px] left-[115px] [font-family:'Jomhuria-Regular',Helvetica] font-normal text-black text-[95px] tracking-[0] leading-[normal] whitespace-nowrap">
        MUSIC AND BAND
      </div>

      <div className="absolute top-[313px] left-[115px] [font-family:'Jomhuria-Regular',Helvetica] font-normal text-black text-[95px] tracking-[0] leading-[normal] whitespace-nowrap">
        DANCING
      </div>

      <div className="absolute top-[443px] left-[115px] [font-family:'Jomhuria-Regular',Helvetica] font-normal text-black text-[95px] tracking-[0] leading-[normal] whitespace-nowrap">
        U1 ENTRY
      </div>

      <div className="absolute top-[512px] left-[115px] [font-family:'Jomhuria-Regular',Helvetica] font-normal text-black text-[95px] tracking-[0] leading-[normal] whitespace-nowrap">
        DJ
      </div>

      <div className="top-[117px] left-[51px] absolute [font-family:'Jomhuria-Regular',Helvetica] font-normal text-black text-[95px] tracking-[0] leading-[normal]">
        *
      </div>

      <div className="top-[454px] left-[54px] absolute [font-family:'Jomhuria-Regular',Helvetica] font-normal text-black text-[95px] tracking-[0] leading-[normal]">
        *
      </div>

      <div className="top-[244px] left-[51px] whitespace-nowrap absolute [font-family:'Jomhuria-Regular',Helvetica] font-normal text-black text-[95px] tracking-[0] leading-[normal]">
        *
      </div>

      <div className="top-[175px] left-[51px] absolute [font-family:'Jomhuria-Regular',Helvetica] font-normal text-black text-[95px] tracking-[0] leading-[normal]">
        *
      </div>

      <div className="top-[385px] left-[51px] absolute [font-family:'Jomhuria-Regular',Helvetica] font-normal text-black text-[95px] tracking-[0] leading-[normal]">
        *
      </div>

      <div className="top-[317px] left-[51px] whitespace-nowrap absolute [font-family:'Jomhuria-Regular',Helvetica] font-normal text-black text-[95px] tracking-[0] leading-[normal]">
        *
      </div>

      <div className="top-[517px] left-[54px] absolute [font-family:'Jomhuria-Regular',Helvetica] font-normal text-black text-[95px] tracking-[0] leading-[normal]">
        *
      </div>

      <div className="absolute top-[707px] left-[61px] w-[378px] [font-family:'Jaro-Regular',Helvetica] font-normal text-black text-[75px] tracking-[0] leading-[normal]">
        DESIGNED
      </div>

      <div className="absolute top-[707px] left-[369px] [font-family:'Jaro-Regular',Helvetica] font-normal text-black text-[75px] tracking-[0] leading-[normal]">
        BY
      </div>

      <div className="absolute top-[813px] left-[142px] [font-family:'Jaro-Regular',Helvetica] font-normal text-black text-[75px] tracking-[0] leading-[normal]">
        AASHIK.A
      </div>
    </div>
  );
};
css
@tailwind components;
@tailwind utilities;

@layer components {
  .all-\[unset\] {
    all: unset;
  }
}

:root {
  --animate-spin: spin 1s linear infinite;
}

.animate-fade-in {
  animation: fade-in 1s var(--animation-delay, 0s) ease forwards;
}

.animate-fade-up {
  animation: fade-up 1s var(--animation-delay, 0s) ease forwards;
}

.animate-marquee {
  animation: marquee var(--duration) infinite linear;
}

.animate-marquee-vertical {
  animation: marquee-vertical var(--duration) linear infinite;
}

.animate-shimmer {
  animation: shimmer 8s infinite;
}

.animate-spin {
  animation: var(--animate-spin);
}

@keyframes spin {
  to {
    transform: rotate(1turn);
  }
}

@keyframes image-glow {
  0% {
    opacity: 0;
    animation-timing-function: cubic-bezier(0.74, 0.25, 0.76, 1);
  }

  10% {
    opacity: 0.7;
    animation-timing-function: cubic-bezier(0.12, 0.01, 0.08, 0.99);
  }

  to {
    opacity: 0.4;
  }
}

@keyframes fade-in {
  0% {
    opacity: 0;
    transform: translateY(-10px);
  }

  to {
    opacity: 1;
    transform: none;
  }
}

@keyframes fade-up {
  0% {
    opacity: 0;
    transform: translateY(20px);
  }

  to {
    opacity: 1;
    transform: none;
  }
}

@keyframes shimmer {
  0%,
  90%,
  to {
    background-position: calc(-100% - var(--shimmer-width)) 0;
  }

  30%,
  60% {
    background-position: calc(100% + var(--shimmer-width)) 0;
  }
}

@keyframes marquee {
  0% {
    transform: translate(0);
  }

  to {
    transform: translateX(calc(-100% - var(--gap)));
  }
}

@keyframes marquee-vertical {
  0% {
    transform: translateY(0);
  }

  to {
    transform: translateY(calc(-100% - var(--gap)));
  }
}
js
/** @type {import('tailwindcss').Config} */
module.exports = {
  content: ["./src/**/*.{html,js,ts,jsx,tsx}"],
  theme: {
    extend: {},
  },
  plugins: [],
};
page3
jsx
import React from "react";

export const IphoneProMax = () => {
  return (
    <div className="bg-white w-full min-w-[604px] min-h-[956px] relative">
      <div className="absolute top-[-62px] left-0 w-[604px] h-[201px] bg-[#00ffff]" />

      <div className="absolute -top-10 left-[19px] [font-family:'Gurajada-Regular',Helvetica] font-normal text-black text-[80px] tracking-[0] leading-[normal]">
        EVENT REGISTRATION
      </div>

      <div className="absolute top-[27px] left-[19px] [font-family:'Gurajada-Regular',Helvetica] font-normal text-black text-[75px] tracking-[0] leading-[normal]">
        FORM
      </div>

      <div className="absolute top-[117px] left-[53px] [font-family:'Gurajada-Regular',Helvetica] font-normal text-black text-[75px] tracking-[0] leading-[normal]">
        FULL NAME
      </div>

      <div className="absolute top-[191px] left-12 [font-family:'Gurajada-Regular',Helvetica] font-normal text-black text-[75px] tracking-[0] leading-[normal]">
        GENDER
      </div>

      <div className="absolute top-[264px] left-[55px] [font-family:'Gurajada-Regular',Helvetica] font-normal text-black text-[75px] tracking-[0] leading-[normal]">
        AGE
      </div>

      <div className="absolute top-[338px] left-[53px] [font-family:'Gurajada-Regular',Helvetica] font-normal text-black text-[75px] tracking-[0] leading-[normal]">
        REGISTER NO
      </div>

      <div className="absolute top-[412px] left-[53px] [font-family:'Gurajada-Regular',Helvetica] font-normal text-black text-[75px] tracking-[0] leading-[normal]">
        DEPARTMENT
      </div>

      <div className="absolute top-[486px] left-[53px] [font-family:'Gurajada-Regular',Helvetica] font-normal text-black text-[75px] tracking-[0] leading-[normal]">
        MOBILE NO
      </div>

      <div className="absolute top-[560px] left-[53px] [font-family:'Gurajada-Regular',Helvetica] font-normal text-black text-[75px] tracking-[0] leading-[normal]">
        EMAIL ID
      </div>

      <div className="absolute top-[631px] left-[55px] [font-family:'Gurajada-Regular',Helvetica] font-normal text-black text-[75px] tracking-[0] leading-[normal]">
        EVENTS
      </div>

      <div className="absolute top-[668px] left-[53px] [font-family:'Gurajada-Regular',Helvetica] font-normal text-black text-[75px] tracking-[0] leading-[normal]">
        REGISTERED
      </div>

      <div className="absolute top-[818px] left-[58px] w-[271px] h-[74px] bg-[#fe1313]" />

      <div className="absolute top-[781px] left-[104px] [font-family:'Gurajada-Regular',Helvetica] font-normal text-black text-[75px] tracking-[0] leading-[normal]">
        SUMBIT
      </div>
    </div>
  );
};
css
@tailwind components;
@tailwind utilities;

@layer components {
  .all-\[unset\] {
    all: unset;
  }
}

:root {
  --animate-spin: spin 1s linear infinite;
}

.animate-fade-in {
  animation: fade-in 1s var(--animation-delay, 0s) ease forwards;
}

.animate-fade-up {
  animation: fade-up 1s var(--animation-delay, 0s) ease forwards;
}

.animate-marquee {
  animation: marquee var(--duration) infinite linear;
}

.animate-marquee-vertical {
  animation: marquee-vertical var(--duration) linear infinite;
}

.animate-shimmer {
  animation: shimmer 8s infinite;
}

.animate-spin {
  animation: var(--animate-spin);
}

@keyframes spin {
  to {
    transform: rotate(1turn);
  }
}

@keyframes image-glow {
  0% {
    opacity: 0;
    animation-timing-function: cubic-bezier(0.74, 0.25, 0.76, 1);
  }

  10% {
    opacity: 0.7;
    animation-timing-function: cubic-bezier(0.12, 0.01, 0.08, 0.99);
  }

  to {
    opacity: 0.4;
  }
}

@keyframes fade-in {
  0% {
    opacity: 0;
    transform: translateY(-10px);
  }

  to {
    opacity: 1;
    transform: none;
  }
}

@keyframes fade-up {
  0% {
    opacity: 0;
    transform: translateY(20px);
  }

  to {
    opacity: 1;
    transform: none;
  }
}

@keyframes shimmer {
  0%,
  90%,
  to {
    background-position: calc(-100% - var(--shimmer-width)) 0;
  }

  30%,
  60% {
    background-position: calc(100% + var(--shimmer-width)) 0;
  }
}

@keyframes marquee {
  0% {
    transform: translate(0);
  }

  to {
    transform: translateX(calc(-100% - var(--gap)));
  }
}

@keyframes marquee-vertical {
  0% {
    transform: translateY(0);
  }

  to {
    transform: translateY(calc(-100% - var(--gap)));
  }
}
js
/** @type {import('tailwindcss').Config} */
module.exports = {
  content: ["./src/**/*.{html,js,ts,jsx,tsx}"],
  theme: {
    extend: {},
  },
  plugins: [],
};


## OUTPUT:

Screenshot 2025-12-28 234636.png
## RESULT:
The program to design, develop and deploy a web application for event registration using Figma UI tool is completed successfully.
