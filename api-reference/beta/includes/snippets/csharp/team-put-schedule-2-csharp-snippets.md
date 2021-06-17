---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 95dc4a32c48394f51264805854bbe3c73dbf26eb
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/17/2021
ms.locfileid: "52992430"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

using var schedule = new System.IO.MemoryStream(Encoding.UTF8.GetBytes(@"{
   ""enabled"":true,
   ""timeZone"":""America/Chicago"",
   ""provisionStatus"":""Completed"",
   ""provisionStatusCode"":null,
   ""openShiftsEnabled"":true,
   ""swapShiftsRequestsEnabled"":true,
   ""offerShiftRequestsEnabled"":true,
   ""timeOffRequestsEnabled"":true,
   ""timeClockEnabled"":true,
   ""timeClockSettings"":{
      ""approvedLocation"":{
         ""altitude"":1024.13,
         ""latitude"":26.13246,
         ""longitude"":24.34616
      }
   }
}"));

await graphClient.Teams["{team-id}"].Schedule
    .Request()
    .PutAsync<Team>(schedule);

```