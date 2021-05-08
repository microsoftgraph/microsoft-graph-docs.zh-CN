---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 541baa00c7a946c8a7c1794ce752c44d5ab2c18c
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52241342"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var deployment = await graphClient.Admin.Windows.Updates.Deployments["{windowsUpdates.deployment-id}"]
    .Request()
    .GetAsync();

```