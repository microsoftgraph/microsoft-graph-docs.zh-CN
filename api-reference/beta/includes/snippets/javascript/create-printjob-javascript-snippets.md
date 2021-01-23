---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4a807f6786f13bf421aafb1f4afefc1bb5425276
ms.sourcegitcommit: 9a5facff47a8d4e05ecd2c6cd68294a948c47c4d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2021
ms.locfileid: "49946019"
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

let res = await client.api('/print/printers/{id}/jobs')
    .version('beta')
    .post(printJob);

```