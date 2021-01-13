---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fbd04e8f7df64462f4a151af4e3b3cb11b50ce49
ms.sourcegitcommit: a9731e19589dcb5c0c6fe2e24b008c86573ef803
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/13/2021
ms.locfileid: "49843582"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var printJobConfiguration = new PrintJobConfiguration
{
    FeedOrientation = PrinterFeedOrientation.LongEdgeFirst,
    PageRanges = new List<IntegerRange>()
    {
        new IntegerRange
        {
            Start = 1,
            End = 1
        }
    },
    Quality = PrintQuality.Medium,
    Dpi = 600,
    Orientation = PrintOrientation.Landscape,
    Copies = 1,
    DuplexMode = PrintDuplexMode.OneSided,
    ColorMode = PrintColorMode.BlackAndWhite,
    InputBin = "by-pass-tray",
    OutputBin = "output-tray",
    MediaSize = "A4",
    Margin = new PrintMargin
    {
        Top = 0,
        Bottom = 0,
        Left = 0,
        Right = 0
    },
    MediaType = "stationery",
    Finishings = null,
    PagesPerSheet = 1,
    MultipageLayout = PrintMultipageLayout.ClockwiseFromBottomLeft,
    Collate = false,
    Scaling = PrintScaling.ShrinkToFit,
    FitPdfToPage = false
};

var jobs = new PrintJob();
jobs.Configuration = printJobConfiguration;

await graphClient.Print.Printers["d5ef6ec4-07ca-4212-baf9-d45be126bfbb"].Jobs["44353"]
    .Request()
    .UpdateAsync(jobs);

```