---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7e3e2c282c807d86decf22a0bf7ef7bedadd72457e419a503ed1ec1b061022e6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333753"
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