---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8268ae953815b194b037cbe3914048733fa41c8a
ms.sourcegitcommit: c47e3d1f3c5f7e2635b2ad29dfef8fe7c8080bc8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/15/2021
ms.locfileid: "61524838"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Users["{user-id}"].Presence
    .ClearUserPreferredPresence()
    .Request()
    .PostAsync();

```