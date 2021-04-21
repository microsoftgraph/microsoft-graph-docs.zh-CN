---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: df2e153ec1e4c6814de2ddcbd7569553a7f74233
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/21/2021
ms.locfileid: "51921947"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var destinationPrinterId = "9a3b3956-ce5b-4d06-a605-5b0bd3e9ddea";

var configuration = new PrintJobConfiguration
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

await graphClient.Print.Printers["{printer-id}"].Jobs["{printJob-id}"]
    .Redirect(destinationPrinterId,configuration)
    .Request()
    .PostAsync();

```