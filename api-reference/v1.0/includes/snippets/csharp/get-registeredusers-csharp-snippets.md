---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9d799fe58215a06e937eaa6ed5b8c1f46d3945e3
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50781311"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var registeredUsers = await graphClient.Devices["{device-id}"].RegisteredUsers
    .Request()
    .GetAsync();

```