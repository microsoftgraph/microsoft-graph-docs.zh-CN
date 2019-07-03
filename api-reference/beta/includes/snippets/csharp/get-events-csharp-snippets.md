---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 95fb59971bf7eab6367331ccd74f2f7c575d3d0d
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35478195"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var events = await graphClient.Me.Events
    .Request()
    .Header("Prefer","outlook.timezone=\"Pacific Standard Time\"")
    .Select( e => new {
             e.Subject,
             e.Body,
             e.BodyPreview,
             e.Organizer,
             e.Attendees,
             e.Start,
             e.End,
             e.Location 
             })
    .GetAsync();

```