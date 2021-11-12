---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bb38190e27d80648da9b2ee9f2764954b5c44547ee145339e905d5c6d281d1bd
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105129"
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

await client.api('/print/shares/{id}/jobs')
    .version('beta')
    .post(printJob);

```