---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a8b6cfec8e43c9e216f5def9029389dc7dd2376f
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50775953"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const printJob = {
  destinationPrinterId: '9a3b3956-ce5b-4d06-a605-5b0bd3e9ddea',
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

await client.api('/print/printers/{printerId}/jobs/{printJobId}/redirect')
    .post(printJob);

```