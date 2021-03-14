---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e9cd228685d0dd51dd5be740989c879587f9630d
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50805825"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var timeOffRequest = await graphClient.Teams["{team-id}"].Schedule.TimeOffRequests["{timeOffRequest-id}"]
    .Request()
    .GetAsync();

```