---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7c4880de667bec69b3cf0b1c4773fb9ababca18d
ms.sourcegitcommit: 9a5facff47a8d4e05ecd2c6cd68294a948c47c4d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2021
ms.locfileid: "49946317"
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

await graphClient.Print.Printers["{id}"].Jobs
    .Request()
    .AddAsync(printJob);

```