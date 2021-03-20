---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8c473cc2018cf8916fab827a6d809b4a8cab1361
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50955610"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var printJob = new PrintJob
{
    Configuration = new PrintJobConfiguration
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
    }
};

await graphClient.Print.Shares["{printerShare-id}"].Jobs
    .Request()
    .AddAsync(printJob);

```