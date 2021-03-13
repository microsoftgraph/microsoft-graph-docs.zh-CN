---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8553a3e35fc9cfa207e033c3345546983c38f70f
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50799905"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var personWebsite = await graphClient.Me.Profile.Websites["{personWebsite-id}"]
    .Request()
    .GetAsync();

```