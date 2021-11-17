---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1ce615a4feb5de75c8f26f9ebb89e9c5961c37df8ba65064ddfe80fa5c45e561
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902467"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var timeCard = new TimeCard
{
    UserId = "70e47528-2fae-42b5-9d8e-ee73ccd90603",
    State = TimeCardState.ClockedOut,
    ConfirmedBy = ConfirmedBy.None,
    Notes = null,
    ClockInEvent = new TimeCardEvent
    {
        DateTime = DateTimeOffset.Parse("2021-05-21T21:58:41.327Z"),
        AtApprovedLocation = null,
        Notes = new ItemBody
        {
            ContentType = BodyType.Text,
            Content = "update sample notes"
        }
    },
    ClockOutEvent = new TimeCardEvent
    {
        DateTime = DateTimeOffset.Parse("2021-05-21T22:01:46.205Z"),
        AtApprovedLocation = null,
        Notes = new ItemBody
        {
            ContentType = BodyType.Text,
            Content = "update sample notes"
        }
    },
    Breaks = new List<TimeCardBreak>()
    {
        new TimeCardBreak
        {
            BreakId = "BRK_138f4751-68b1-44c1-aca2-2b26cba9e73f",
            Notes = null,
            Start = new TimeCardEvent
            {
                DateTime = DateTimeOffset.Parse("2021-05-21T21:59:59.328Z"),
                AtApprovedLocation = null,
                Notes = new ItemBody
                {
                    ContentType = BodyType.Text,
                    Content = "update sample notes"
                }
            },
            End = new TimeCardEvent
            {
                DateTime = DateTimeOffset.Parse("2021-05-21T22:01:10.205Z"),
                AtApprovedLocation = null,
                Notes = new ItemBody
                {
                    ContentType = BodyType.Text,
                    Content = "update sample notes"
                }
            }
        }
    }
};

await graphClient.Teams["{team-id}"].Schedule.TimeCards["{timeCard-id}"]
    .Request()
    .PutAsync(timeCard);

```