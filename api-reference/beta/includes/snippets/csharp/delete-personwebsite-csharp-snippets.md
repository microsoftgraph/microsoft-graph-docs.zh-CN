---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 04ea0a988de2a1baa608b6fd77c486fdd0f10d40
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50796552"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Profile.Websites["{personWebsite-id}"]
    .Request()
    .DeleteAsync();

```