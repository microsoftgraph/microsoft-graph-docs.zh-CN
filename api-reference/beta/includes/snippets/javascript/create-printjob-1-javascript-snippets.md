---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: adc0dc839774a4f0c2e32248e153ab537cef8f4a
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50955666"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const printJob = {
  configuration: {
    feedOrientation: 'longEdgeFirst',
    pageRanges: [
      {
        start: 1,
        end: 1
      }
    ],
    quality: 'medium',
    dpi: 600,
    orientation: 'landscape',
    copies: 1,
    duplexMode: 'oneSided',
    colorMode: 'blackAndWhite',
    inputBin: 'by-pass-tray',
    outputBin: 'output-tray',
    mediaSize: 'A4',
    margin: {
      top: 0,
      bottom: 0,
      left: 0,
      right: 0
    },
    mediaType: 'stationery',
    finishings: null,
    pagesPerSheet: 1,
    multipageLayout: 'clockwiseFromBottomLeft',
    collate: false,
    scaling: 'shrinkToFit',
    fitPdfToPage: false
  }
};

await client.api('/print/printers/{id}/jobs')
    .version('beta')
    .post(printJob);

```