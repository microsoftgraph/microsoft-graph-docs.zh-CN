---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: abe3a4cd6a4ff6c7b4670ed6b91cee372f1757ab2ed4f5e0155f142abc974090
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903859"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var timeOffReason = new TimeOffReason
{
    DisplayName = "Vacation",
    IconType = TimeOffReasonIconType.Plane,
    IsActive = true
};

await graphClient.Teams["{team-id}"].Schedule.TimeOffReasons["{timeOffReason-id}"]
    .Request()
    .Header("Prefer","return=representation")
    .PutAsync(timeOffReason);

```