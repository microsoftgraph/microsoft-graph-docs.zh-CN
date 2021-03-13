---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c58d6787facd0b30fbb4887540e99161a3766a2a
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50768756"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrintJob printJob = new PrintJob();
PrintJobConfiguration configuration = new PrintJobConfiguration();
configuration.feedOrientation = PrinterFeedOrientation.LONG_EDGE_FIRST;
LinkedList<IntegerRange> pageRangesList = new LinkedList<IntegerRange>();
IntegerRange pageRanges = new IntegerRange();
pageRanges.start = 1L;
pageRanges.end = 1L;
pageRangesList.add(pageRanges);
configuration.pageRanges = pageRangesList;
configuration.quality = PrintQuality.MEDIUM;
configuration.dpi = 600;
configuration.orientation = PrintOrientation.LANDSCAPE;
configuration.copies = 1;
configuration.duplexMode = PrintDuplexMode.ONE_SIDED;
configuration.colorMode = PrintColorMode.BLACK_AND_WHITE;
configuration.inputBin = "by-pass-tray";
configuration.outputBin = "output-tray";
configuration.mediaSize = "A4";
PrintMargin margin = new PrintMargin();
margin.top = 0;
margin.bottom = 0;
margin.left = 0;
margin.right = 0;
configuration.margin = margin;
configuration.mediaType = "stationery";
configuration.finishings = null;
configuration.pagesPerSheet = 1;
configuration.multipageLayout = PrintMultipageLayout.CLOCKWISE_FROM_BOTTOM_LEFT;
configuration.collate = false;
configuration.scaling = PrintScaling.SHRINK_TO_FIT;
configuration.fitPdfToPage = false;
printJob.configuration = configuration;

graphClient.print().printers("{printerId}").jobs("{printJobId}")
    .buildRequest()
    .patch(printJob);

```