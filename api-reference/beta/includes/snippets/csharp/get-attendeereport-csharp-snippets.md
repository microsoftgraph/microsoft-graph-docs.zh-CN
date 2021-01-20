---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: be8bdd1645fd71c2ba4a592180cd4aece86b37b1
ms.sourcegitcommit: 6314172db76ba9f2c192d8c099d818c5e772d2b8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2021
ms.locfileid: "49910878"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var stream = await graphClient.Users["dc74d9bb-6afe-433d-8eaa-e39d80d3a647"].OnlineMeetings["dc17674c-81d9-4adb-bfb2-8f6a442e4622_19:meeting_ZWE0YzQwMzItYjEyNi00NjJjLWE4MjYtOTUxYjE1NmFjYWIw@thread.v2"].AttendeeReport
    .Request()
    .GetAsync();

```