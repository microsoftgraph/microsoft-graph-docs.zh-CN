---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bf642af2e0b45346cc37bac7e9577855d1540484
ms.sourcegitcommit: a9731e19589dcb5c0c6fe2e24b008c86573ef803
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/13/2021
ms.locfileid: "49843586"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const printJobConfiguration = {
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
};

let res = await client.api('/print/printers/d5ef6ec4-07ca-4212-baf9-d45be126bfbb/jobs/44353/configuration')
    .version('beta')
    .update(printJobConfiguration);

```