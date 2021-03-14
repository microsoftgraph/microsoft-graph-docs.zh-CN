---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 77086217e4b6f076efc47292fbe67b9504ced7de
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50789454"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var group = await graphClient.Groups["{group-id}"]
    .Request()
    .Select("allowExternalSenders,autoSubscribeNewMembers,isSubscribedByMail,unseenCount")
    .GetAsync();

```