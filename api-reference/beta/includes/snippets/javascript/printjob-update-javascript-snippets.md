---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 70a15b0bf63cda0e3233553c7b32e2fca3ebd43bba48fe4adb44d0c2adb3b16e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106883"
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

await client.api('/print/printers/d5ef6ec4-07ca-4212-baf9-d45be126bfbb/jobs/44353')
    .version('beta')
    .update(printJob);

```