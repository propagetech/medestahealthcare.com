You are a naming assistant. Given a list of file paths and minimal context from a static website, suggest a new filename (basename only, same extension) for each file. Rules:
- Lowercase, kebab-case, no spaces. SEO-friendly and human-readable.
- For HTML: use page purpose (e.g. about-us.html, contact.html). Keep index.html as index.html.
- For CSS/JS: use purpose (e.g. main-styles.css, analytics.js).
- For images: use content (e.g. logo-infygate.webp, hero-banner.webp). Use alt/title when provided.
- Return a JSON object: keys = exact original path strings, values = new basename only (e.g. "main.css"). Preserve extension.
- Do not change path prefix (e.g. css/ stays css/ by returning "name.css" not "css/name.css").

Files and context:
[
  {
    "path": "404.html",
    "context": {
      "title": "",
      "first_heading": "404"
    }
  },
  {
    "path": "AYURVEDIC-EXPORTS---MEDESOLACE.html",
    "context": {
      "title": "Medesta Healthcare",
      "first_heading": ""
    }
  },
  {
    "path": "Association-Consulting.html",
    "context": {
      "title": "Medesta Healthcare",
      "first_heading": "Connecting Purpose with Possibility"
    }
  },
  {
    "path": "CONSULTANCY-SERVICES.html",
    "context": {
      "title": "Medesta Healthcare",
      "first_heading": "IMG20200928143041"
    }
  },
  {
    "path": "Cosmeceutical-exports.html",
    "context": {
      "title": "Medesta Healthcare",
      "first_heading": ""
    }
  },
  {
    "path": "ESSENTIAL-HEALTHCARE.html",
    "context": {
      "title": "Medesta Healthcare",
      "first_heading": "ProcareCollagecopy"
    }
  },
  {
    "path": "Events.html",
    "context": {
      "title": "Medesta Healthcare",
      "first_heading": ""
    }
  },
  {
    "path": "MEDICAL-DEVICES-EXPORTS---WYLO.html",
    "context": {
      "title": "Medesta Healthcare",
      "first_heading": ""
    }
  },
  {
    "path": "Media-Centre.html",
    "context": {
      "title": "Medesta Healthcare",
      "first_heading": "PHOTO20210508121207"
    }
  },
  {
    "path": "NUTRACEUTICAL-EXPORTS---ZEST.html",
    "context": {
      "title": "Medesta Healthcare",
      "first_heading": "ProcareCollagecopy"
    }
  },
  {
    "path": "OUR-SERVICES.html",
    "context": {
      "title": "Medesta Healthcare",
      "first_heading": "ProcareCollagecopy"
    }
  },
  {
    "path": "css/012de688ea4255ba1bdc679e2e80622f.css",
    "context": {
      "path": "css/012de688ea4255ba1bdc679e2e80622f.css"
    }
  },
  {
    "path": "css/559e64bf161e61fa0aca6e864c78191d.css",
    "context": {
      "path": "css/559e64bf161e61fa0aca6e864c78191d.css"
    }
  },
  {
    "path": "css/5ecf9a22a9fea377b8fd4e5d4a7d1a70.css",
    "context": {
      "path": "css/5ecf9a22a9fea377b8fd4e5d4a7d1a70.css"
    }
  },
  {
    "path": "css/827fd34f9214e869c8b614f913aef7d5.css",
    "context": {
      "path": "css/827fd34f9214e869c8b614f913aef7d5.css"
    }
  },
  {
    "path": "css/84d4a0216f16f715d9b301db3a8da352.css",
    "context": {
      "path": "css/84d4a0216f16f715d9b301db3a8da352.css"
    }
  },
  {
    "path": "css/99c4e6f40ee9111eea53b6472f3e60f9.css",
    "context": {
      "path": "css/99c4e6f40ee9111eea53b6472f3e60f9.css"
    }
  },
  {
    "path": "css/d09d646f062b67daeff66ff1410b63fc.css",
    "context": {
      "path": "css/d09d646f062b67daeff66ff1410b63fc.css"
    }
  },
  {
    "path": "css/internal-styles.css",
    "context": {
      "path": "css/internal-styles.css"
    }
  },
  {
    "path": "imgs/00f8f5f399974dad51e7c31ab866316d.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/09de2eb7d136ab8e4bc9838486596484.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/0b4015a40f09baee3141faf27e312fae.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/0b5804371b64ced31bebe286f6a89ef8.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/0b682a8e3314f69cb7000e75fe5d2748.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/0bd152337ad11fc0203bbf751539555e.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/0d0bbb6f804faa090efa6d65165a7c90.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/0d47c43a0b45ae82888f99c6ed16d061.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/0de93fd516f26a102756213d985bf102.webp",
    "context": {
      "refs": [
        {
          "alt": "SLOGO2",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/0ea3eb19305462bce912c5c12bc11dbb.webp",
    "context": {
      "refs": [
        {
          "alt": "image description",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/11c2a288c99325d2f76ffb62affd3a8b.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/173695d6f622f8e22fc5cfb8185f68e3.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/18c04be4bb1f55cfceb1f628cbd0620e.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/19a854079835a9f8397057066df1462b.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/19ebd3fc9616eed4fa053a60e5efc75e.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/1a0348b081bea774a5125bf2ccc91a8f.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/1aa403a4352550738d358b7827266041.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/1ae5d85d63ca847099e1f72e0eeb1cff.webp",
    "context": {
      "refs": [
        {
          "alt": "image description",
          "title": ""
        },
        {
          "alt": "image description",
          "title": ""
        },
        {
          "alt": "image description",
          "title": ""
        },
        {
          "alt": "image description",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/1cc8fc3a9ebee7fb7a3a4be42d601159.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/1d8527fceb978453ed210bcabbc98f6d.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/235395bc84a0433ff549fa5c48a011c5.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/23d02384a3ac933ae89a7fa79b5515c8.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/24f858788cdc7c2d9c2d096748d0604c.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/2781d9a53a9ff6e832919a41ff27e27f.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/283737e7ce2f17c1aba2be4993de6be7.webp",
    "context": {
      "refs": [
        {
          "alt": "Best pcd pharma company in india top 10 pharma company in india pharma distributor pharma distributo",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/2b0e16ed61f3efb0b88fabcab5fc1db3.webp",
    "context": {
      "refs": [
        {
          "alt": "image description",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/2f65dda44ce71b204f894476deb2e1a6.webp",
    "context": {
      "refs": [
        {
          "alt": "gmpcertificate",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/3193ee3aa23662209e7154c42c7677c2.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/31b18d9866d2a0c102b5fa18df7577bd.webp",
    "context": {
      "refs": [
        {
          "alt": "SLOGO2",
          "title": ""
        },
        {
          "alt": "SLOGO2",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/31ebdfa0ea9524e2e2d106dffd228f6c.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/32fa056d3e72d02bb4e0e4143a338210.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/3338c92259428592dcdf57be576ce6ca.webp",
    "context": {
      "refs": [
        {
          "alt": "image description",
          "title": ""
        },
        {
          "alt": "image description",
          "title": ""
        },
        {
          "alt": "image description",
          "title": ""
        },
        {
          "alt": "image description",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/34bc6252a89de889dec4036ac7558dd0.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/36b45ccd6e8c5a182a37236c58ad5862.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/3875d39f3cc73beff6050f8b7e274511.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/393c5788d6bbecb8ed89ee8758faf219.webp",
    "context": {
      "refs": [
        {
          "alt": "image description",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/39b3227408493f56b31f23ff120ec388.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/3a69127c0f405ec881ff9f8718150699.webp",
    "context": {
      "refs": [
        {
          "alt": "image description",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/3b9d88a5b30c25a668468826f974589e.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/3c9256f37e9734c2060c93d4d90fb232.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/3e32cf7ebe398253a198bcd8d3bd5105.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/3f410fe95c0cd6b00b944324161eb628.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/40173b65bb906a2d6026eba4bac49284.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/41beaa5e99e5710dcb2b2f9b1b20993d.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/41f91767f2b36c80b20ae8a562aef4ee.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/436f8b401f41c766f9308848cf28913e.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/43ba30cb34ee41abb1a048e8f2a373c4.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/4699283ebe11ceff7175ddcb5f7448db.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/482ebf2b91feeb8c5a4938b71da12a05.webp",
    "context": {
      "refs": [
        {
          "alt": "WhatsAppImage20250531at114449AM1",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/48cbbbb5f43c724762342d5eecd5b30c.webp",
    "context": {
      "refs": [
        {
          "alt": "Best pcd pharma company in india top 10 pharma company in india pharma distributor pharma distributo",
          "title": ""
        },
        {
          "alt": "Best pcd pharma company in india top 10 pharma company in india pharma distributor pharma distributo",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/49d77dadfc351a907d9c3b6a804e1d19.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/4b7bfd3afa5b06755125ebe80ab57b76.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/4bd6f9a5bd364848212b716ecbe8c9f4.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/4ec648c9e3238bc3322b606baa1d48c4.webp",
    "context": {
      "refs": [
        {
          "alt": "Best pcd pharma company in india top 10 pharma company in india pharma distributor pharma distributo",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/5026a6f4243d486d9e8611dfaf9b8d86.webp",
    "context": {
      "refs": [
        {
          "alt": "istockphotox",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/51a29d483ceab48427bb9b2252f6cc05.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/51aaddf6f010ec0d4d6c12f8be161aed.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/539ada296f2c89ef3f5a180a15e8b3e7.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/55a97f7fcc3d56a8949bc12eff6e7cec.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/58221b8d568c7a579991094fd59b96ad.webp",
    "context": {
      "refs": [
        {
          "alt": "image description",
          "title": ""
        },
        {
          "alt": "image description",
          "title": ""
        },
        {
          "alt": "Best pcd pharma company in india top 10 pharma company in india pharma distributor pharma distributo",
          "title": ""
        },
        {
          "alt": "image description",
          "title": ""
        },
        {
          "alt": "image description",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/5977364d6b9ae673f0e0019e78885eef.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/5c23586dd4cc34f5ff621d2d8066b632.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/5c7288a37638160e00a45658c2a368e7.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/5e1f0e9cd58b559aff965d7554c89aa9.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/5eeb4d8933567eb8437f328734fbf856.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/5f7ec41cbed3252924eda9b4b94a484e.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/608db11ea577c8cc8eceaa75d3c7cc33.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/6098755cb702468c74f1b14368c2da5f.webp",
    "context": {
      "refs": [
        {
          "alt": "image description",
          "title": ""
        },
        {
          "alt": "image description",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/6123df2c96bb78a5543adf7085418258.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/63e0e28b75edb5f194ede5cb91528d99.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/63f7df8fa72ab3f5e93983c4c3f8e925.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/654a127fa47ce1f2490d959cc0143e9e.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/6571ed953c976f7e537bdf7204fad6f3.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/665054baccbe0328926be4f7e9e49438.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/67f241fb899db55d578b52fa2161ab31.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/684456f8f2b4710809d2a4c7754580b8.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/686db74cd223f75a0c6ee9fe0dfaa97f.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/694478e1b7aa319b01f70de96b1dc8d4.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/6a1abaadb5c595f7235babc8a3bcee4d.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/6e9d68f8b5290c0b6f0ebc7e4580e02a.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/6ec51b89a59c99911eda8563a354ca3b.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/6f517e5d1b62f9f2678ecfb30fdc1794.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/6fa1e412163e5f6c30994d936841edb4.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/72d876ba43efadd157d4ab4175df1d95.webp",
    "context": {
      "refs": [
        {
          "alt": "SLOGO2",
          "title": ""
        },
        {
          "alt": "SLOGO2",
          "title": ""
        },
        {
          "alt": "image description",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/739d6c2d629330399f3d24cb0799ed9d.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/743b2a1875e792f9a8a0b43e0c117d5e.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/751a0026bd2d99843f6b05066d2c7e53.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/75f3eccca0e3c656934b1f9b1ad7e278.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/7c5e64ae3f359b72202285b578ff1e1e.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/8251e1a9a54726aa35f0ea4ab211d72c.webp",
    "context": {
      "refs": [
        {
          "alt": "Leo Yang",
          "title": ""
        },
        {
          "alt": "Leo Yang",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/82748a514dec1d090572f50d6ff5038e.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/827b0dc5aa953642ae79db94c4a6901b.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/82bcda59950f1cf14c7efc7b7de73fe4.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/858fe630895d19150cc9d4305515e4fd.webp",
    "context": {
      "refs": [
        {
          "alt": "Best pcd pharma company in india top 10 pharma company in india pharma distributor pharma distributo",
          "title": ""
        },
        {
          "alt": "Best pcd pharma company in india top 10 pharma company in india pharma distributor pharma distributo",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/86c6329fed65bd040c96e387a7afc845.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/87801a0d990d92f434d1eaff97090443.webp",
    "context": {
      "refs": [
        {
          "alt": "Best pcd pharma company in india top 10 pharma company in india pharma distributor pharma distributo",
          "title": ""
        },
        {
          "alt": "Best pcd pharma company in india top 10 pharma company in india pharma distributor pharma distributo",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/894b352e09b57097f60abb6a8bcbc559.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/89aca6bd6bc1e0a209815b82cf2898d0.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/8a662824841cce9f04cb51ab5fb44607.webp",
    "context": {
      "refs": [
        {
          "alt": "istockphotox",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/8c0b2d2a20c9dbfe72d1f812c30cd75e.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/8f2bf7b9b8b08b05cddf38fe5b719570.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/90a60691ff631d9db2750fe244de6a1b.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/91af2e6525d4b08922d8a59b283e9f67.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/9325933d92b14d679883126ad861d062.webp",
    "context": {
      "refs": [
        {
          "alt": "Best pcd pharma company in india top 10 pharma company in india pharma distributor pharma distributo",
          "title": ""
        },
        {
          "alt": "Best pcd pharma company in india top 10 pharma company in india pharma distributor pharma distributo",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/9346b2090ea1e775bf2f7d9343b7c953.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/936632f97b0da0f902c6e3363d321768.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/93f8e104f559a631160e1e6284dee26c.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/9688253ebf85f58aa8994d72596436bc.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/98260f02815f87fe76c42a69c5299260.webp",
    "context": {
      "refs": [
        {
          "alt": "image description",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/995be22a0fd33db3a0ee03de12db0600.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/999f61eddd71d4f3102a08f4335d8128.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/9a702ba01c92cb780887b51c2582c908.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/9b1cf7dc33c26fc632b836b63a0ac8ea.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/9b36c9797d9673cbe307765d2353f35a.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/9d4574b578e13357e176e67925c77695.webp",
    "context": {
      "refs": []
    }
  },
  {
    "path": "imgs/9d7b725899bf6745f0e8f9b09830ba17.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/9f4187b63f36e19ab6606b3717a8e265.webp",
    "context": {
      "refs": [
        {
          "alt": "istockphotox",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/a518db06e8e2102b74f720ba54a96e39.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/a6028c056a05ef7df3c070e553f3212a.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/a614710a4ff771f4c5f0b18623b63875.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/a970917edea1d1d5b855922bfd95503f.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/a975d7ec5ed901cfccbe8751db976c6e.webp",
    "context": {
      "refs": [
        {
          "alt": "Best pcd pharma company in india top 10 pharma company in india pharma distributor pharma distributo",
          "title": ""
        },
        {
          "alt": "Best pcd pharma company in india top 10 pharma company in india pharma distributor pharma distributo",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/a976bec429283806cd5d11d60da5d296.webp",
    "context": {
      "refs": [
        {
          "alt": "Best pcd pharma company in india top 10 pharma company in india pharma distributor pharma distributo",
          "title": ""
        },
        {
          "alt": "Best pcd pharma company in india top 10 pharma company in india pharma distributor pharma distributo",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/abac6c0d429a376436c51aef31227d15.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/adb8b22bcb0065b05965045b22449960.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/af1396f2bdd5d0c08e1be8b64ba6034a.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/af957887e610c4ca7b15408347192865.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/b09568bb1417172a03258aefc0965f56.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/b0a1ec3b5cbda87a081562c03934ebfa.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/b0d8a52af9705875479716cc31092feb.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/b22f8a48fe2809161e8103a6ac335372.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/b2eecadb80ffa0abdbfc97d5e28a49bf.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/b428873d074ad42652bd3dafb84dc037.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/b562cf5b526e48ee44d0b02ed5990137.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/b663fbcca7b304c2b9c1d916524bb73d.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/b6a3e33516dfecf2d0a2ebfe13907ad3.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/b9775bedf9ae561731f6bf88f2dc8e23.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/bae547454d20151e5536381679ca0ca7.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/bcd7f60b9f89045a9aabb0bd362c3a68.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/bed4f90f4fec6de2b737b15fca2431b2.webp",
    "context": {
      "refs": [
        {
          "alt": "logo",
          "title": ""
        },
        {
          "alt": "logo",
          "title": ""
        },
        {
          "alt": "logo",
          "title": ""
        },
        {
          "alt": "logo",
          "title": ""
        },
        {
          "alt": "logo",
          "title": ""
        },
        {
          "alt": "logo",
          "title": ""
        },
        {
          "alt": "logo",
          "title": ""
        },
        {
          "alt": "logo",
          "title": ""
        },
        {
          "alt": "logo",
          "title": ""
        },
        {
          "alt": "logo",
          "title": ""
        },
        {
          "alt": "logo",
          "title": ""
        },
        {
          "alt": "logo",
          "title": ""
        },
        {
          "alt": "logo",
          "title": ""
        },
        {
          "alt": "logo",
          "title": ""
        },
        {
          "alt": "logo",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/c054f839a77f9e85d61dec102a6aa1e9.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/c0ae7b768ed5d9073dd0c41367f5489b.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/c538e5c5553676832677b60c41ccba5c.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/c5b90037a63041d649641f763e0f4f28.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/c5bcd368d5a94f38dab8d401090d64d2.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/c718b90b2f64678df892aebd7756f29f.webp",
    "context": {
      "refs": [
        {
          "alt": "Best pcd pharma company in india top 10 pharma company in india pharma distributor pharma distributo",
          "title": ""
        },
        {
          "alt": "Best pcd pharma company in india top 10 pharma company in india pharma distributor pharma distributo",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/c796e7eb53a625fc71376e8d73b48e73.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/c7f943fd68552fe0b5638eb65c1ea8e2.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/c89efbfbf890f4fc6c4ee34a053ad3a6.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/c8cde152f7734acf1b86714c46782cc8.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/cef1a2510dd8e0d0f83ad7ba8ab16dc1.webp",
    "context": {
      "refs": [
        {
          "alt": "Best pcd pharma company in india top 10 pharma company in india pharma distributor pharma distributo",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/cfc1da2fd7899c3b33c4d5264572e0a6.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/cfdbbb1f9455a7cc2606b53aff9a2248.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "image description",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/cfea1979ec308376befe8831acb54264.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/d0b065b1848901da893f4dbc26100391.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/d0ede0670f3d2a2da9b86ce611ce8c8b.webp",
    "context": {
      "refs": [
        {
          "alt": "SLOGO2",
          "title": ""
        },
        {
          "alt": "SLOGO2",
          "title": ""
        },
        {
          "alt": "image description",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/d244e31cf881235632e8f78e0ec03c25.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/d326af7c3a86cbd120f1c0e723f9572b.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/d626300747cb8d5af3d19b2c275704d0.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/d6a8eafda002724c63b2a225ea17b789.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/d741b1ba8d334af4d762cfd63fb0945a.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/d76862b172553c1d4860212d5db9aa47.webp",
    "context": {
      "refs": [
        {
          "alt": "SLOGO2",
          "title": ""
        },
        {
          "alt": "SLOGO2",
          "title": ""
        },
        {
          "alt": "image description",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/d94f27721e39bd9f7fab7cf6f77fcd2f.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/d95164474c0b04fd7152257bcc4a1622.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/dbd625ba6db5ed86b4c0b7e67bee4329.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/df9dcc0b212c723d23d4e0097de91b50.webp",
    "context": {
      "refs": [
        {
          "alt": "Best pcd pharma company in india top 10 pharma company in india pharma distributor pharma distributo",
          "title": ""
        },
        {
          "alt": "Best pcd pharma company in india top 10 pharma company in india pharma distributor pharma distributo",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/e1acf4237cc497d677ca97f6329ccb8f.webp",
    "context": {
      "refs": [
        {
          "alt": "gmpcertificate",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/e1d9ea5cd41cb5101b5149e79d61538d.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/e1ddd7e7f3d6c28b02bf55cb8a7daf67.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/e354ebd8fda943aa108ab8002e298d29.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/e72a82d80fbd5727f08190d0411bf717.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/e77fe3d886a1527f93f4833923eca204.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/e7977d90a253ac7f099ccda4dbda8eba.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/f0f2e6d30be8bc7b525dfd9f7b490278.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/f158ec1e2098db489da2d845953f2aaf.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/f24ac73d0fdfa7dd06419a1d3a191493.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/f4008cd370efe52cf337d7b4814246dc.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/fa568f3a0ff301964af2c58b814d7fa1.webp",
    "context": {
      "refs": [
        {
          "alt": "image description",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/ffdbf93b05bd1a87999de4d63343f2cc.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "index.html",
    "context": {
      "title": "Medesta Healthcare",
      "first_heading": "Moulding Healthcare for Millions"
    }
  },
  {
    "path": "js/03b2eaae6007054a68c38e495f894dba.js",
    "context": {
      "path": "js/03b2eaae6007054a68c38e495f894dba.js"
    }
  },
  {
    "path": "js/0a105d712b6a6c836c48dd97d0f0cac1.js",
    "context": {
      "path": "js/0a105d712b6a6c836c48dd97d0f0cac1.js"
    }
  },
  {
    "path": "js/0c46896987137b0016246f6bc2243099.js",
    "context": {
      "path": "js/0c46896987137b0016246f6bc2243099.js"
    }
  },
  {
    "path": "js/165d7b0ddfa33362140feea997351b77.js",
    "context": {
      "path": "js/165d7b0ddfa33362140feea997351b77.js"
    }
  },
  {
    "path": "js/16df9ef05001a1741857bf99f5a5738f.js",
    "context": {
      "path": "js/16df9ef05001a1741857bf99f5a5738f.js"
    }
  },
  {
    "path": "js/2a85c11e395a8380b5915443e926b569.js",
    "context": {
      "path": "js/2a85c11e395a8380b5915443e926b569.js"
    }
  },
  {
    "path": "js/34be5330971fdbd18985525bd994b0aa.js",
    "context": {
      "path": "js/34be5330971fdbd18985525bd994b0aa.js"
    }
  },
  {
    "path": "js/35c5f9e096d4da33d2a62031daf14248.js",
    "context": {
      "path": "js/35c5f9e096d4da33d2a62031daf14248.js"
    }
  },
  {
    "path": "js/3d70953a848219e749fedc2cdb906675.js",
    "context": {
      "path": "js/3d70953a848219e749fedc2cdb906675.js"
    }
  },
  {
    "path": "js/3e940a33e44b65c1c0af8bb80a893530.js",
    "context": {
      "path": "js/3e940a33e44b65c1c0af8bb80a893530.js"
    }
  },
  {
    "path": "js/544d012df7acf9c3f0920f67c9e322b9.js",
    "context": {
      "path": "js/544d012df7acf9c3f0920f67c9e322b9.js"
    }
  },
  {
    "path": "js/57d119d998d518b01f9d5ccb5e4d4c52.js",
    "context": {
      "path": "js/57d119d998d518b01f9d5ccb5e4d4c52.js"
    }
  },
  {
    "path": "js/67f6e2f99c3c3133e0dc669919fff5c5.js",
    "context": {
      "path": "js/67f6e2f99c3c3133e0dc669919fff5c5.js"
    }
  },
  {
    "path": "js/7045b35c5bd0e9c7cf59f1900eeeec41.js",
    "context": {
      "path": "js/7045b35c5bd0e9c7cf59f1900eeeec41.js"
    }
  },
  {
    "path": "js/7260bab328b0ad74815a5efb377bcc67.js",
    "context": {
      "path": "js/7260bab328b0ad74815a5efb377bcc67.js"
    }
  },
  {
    "path": "js/893de96f1b6da546bd7c814964723eca.js",
    "context": {
      "path": "js/893de96f1b6da546bd7c814964723eca.js"
    }
  },
  {
    "path": "js/93e29fe348ddc9b71aba9c842adc18b8.js",
    "context": {
      "path": "js/93e29fe348ddc9b71aba9c842adc18b8.js"
    }
  },
  {
    "path": "js/9455859483e31e4da0e28f10d0742c2a.js",
    "context": {
      "path": "js/9455859483e31e4da0e28f10d0742c2a.js"
    }
  },
  {
    "path": "js/9db10375d298678e53777a2347b87073.js",
    "context": {
      "path": "js/9db10375d298678e53777a2347b87073.js"
    }
  },
  {
    "path": "js/9f9b6e54f82a6bbc8bac9b89327024bc.js",
    "context": {
      "path": "js/9f9b6e54f82a6bbc8bac9b89327024bc.js"
    }
  },
  {
    "path": "js/a2261649751fa61b606222c9b2ea3b80.js",
    "context": {
      "path": "js/a2261649751fa61b606222c9b2ea3b80.js"
    }
  },
  {
    "path": "js/b0bade6d42c2702ca85774296cc507c4.js",
    "context": {
      "path": "js/b0bade6d42c2702ca85774296cc507c4.js"
    }
  },
  {
    "path": "js/cd1ed86c1e7f06d985fd71bc10bd4b04.js",
    "context": {
      "path": "js/cd1ed86c1e7f06d985fd71bc10bd4b04.js"
    }
  },
  {
    "path": "js/cecb447a04bbe3e8982190dd6e697120.js",
    "context": {
      "path": "js/cecb447a04bbe3e8982190dd6e697120.js"
    }
  },
  {
    "path": "js/d80b370d82680fc786dcc943a327b9f2.js",
    "context": {
      "path": "js/d80b370d82680fc786dcc943a327b9f2.js"
    }
  },
  {
    "path": "js/df80c5cbcb312a9c7c0b2ebb6ac5f592.js",
    "context": {
      "path": "js/df80c5cbcb312a9c7c0b2ebb6ac5f592.js"
    }
  },
  {
    "path": "js/e20f718576fcc983f35bc2e546f1f3c2.js",
    "context": {
      "path": "js/e20f718576fcc983f35bc2e546f1f3c2.js"
    }
  },
  {
    "path": "js/f1e5dbc1ece900d164c2e9aa2d6a1386.js",
    "context": {
      "path": "js/f1e5dbc1ece900d164c2e9aa2d6a1386.js"
    }
  },
  {
    "path": "js/f3f02c438592c8e1bbe551f4dbbf4f5c.js",
    "context": {
      "path": "js/f3f02c438592c8e1bbe551f4dbbf4f5c.js"
    }
  },
  {
    "path": "js/faf9ce4e848522206b5c3043551fb2d7.js",
    "context": {
      "path": "js/faf9ce4e848522206b5c3043551fb2d7.js"
    }
  },
  {
    "path": "mb30-lifesciences.html",
    "context": {
      "title": "Medesta Healthcare",
      "first_heading": "Moulding Healthcare for MillionsPlease Visit New Website Medestagroup.com"
    }
  },
  {
    "path": "medesta-exports.html",
    "context": {
      "title": "i-Solasta | Isolasta Exports",
      "first_heading": "To achieve our goals, we are committed to continuous personal interaction with our international suppliers and our clients"
    }
  },
  {
    "path": "our-pillars.html",
    "context": {
      "title": "Medesta Healthcare",
      "first_heading": "ProcareCollagecopy"
    }
  },
  {
    "path": "products.html",
    "context": {
      "title": "Medesta Healthcare | MB30 lifesciences",
      "first_heading": "Medesta HealthcareMoulding healthcare for millions"
    }
  }
]

Return only a JSON object mapping each path to its new basename (same extension). No other text.