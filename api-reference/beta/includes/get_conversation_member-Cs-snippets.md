---
description: 自动生成的文件。 不修改
ms.openlocfilehash: f0023d2a430b9edda902b8e22ad49161b82cc528
ms.sourcegitcommit: c0df90d66cb2072848d4bb0bf730c47a601b99ce
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/29/2019
ms.locfileid: "34546603"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var members = await graphClient.Me.Chats["{id}"].Members
    .Request()
    .GetAsync();

```