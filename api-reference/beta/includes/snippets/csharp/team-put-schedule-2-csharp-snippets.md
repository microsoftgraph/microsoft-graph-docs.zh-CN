---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e101f878fd47175fb17a24b3b1a87311a35e1e4d617c28859e383647b4f904da
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57103931"
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