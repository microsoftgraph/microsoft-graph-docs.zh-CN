---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 72fdf665214ad82ddfa7c7e53b2e4c5b5d4e65c4
ms.sourcegitcommit: 60ced1be6ed8dd2d23263090a1cfbc16689bb043
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/28/2020
ms.locfileid: "48782733"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const printJob = {
  configuration: {
    feedOrientation: "longEdgeFirst",
    pageRanges: [
      {
        start: 1,
        end: 1
      }
    ],
    quality: "medium",
    dpi: 600,
    orientation: "landscape",
    copies: 1,
    duplexMode: "oneSided",
    colorMode: "blackAndWhite",
    inputBin: "by-pass-tray",
    outputBin: "output-tray",
    mediaSize: "A4",
    margin: {
      top: 0,
      bottom: 0,
      left: 0,
      right: 0
    },
    mediaType: "stationery",
    finishings: null,
    pagesPerSheet: 1,
    multipageLayout: "clockwiseFromBottomLeft",
    collate: false,
    scaling: "shrinkToFit",
    fitPdfToPage: false
  }
};

let res = await client.api('/print/shares/{id}/jobs')
    .version('beta')
    .post(printJob);

```