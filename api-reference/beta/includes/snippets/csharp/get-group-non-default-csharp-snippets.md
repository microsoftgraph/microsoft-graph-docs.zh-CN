---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6597d68c58d32557e26ee2e67c2fda046c1b0f66
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2020
ms.locfileid: "44685072"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var group = await graphClient.Groups["b320ee12-b1cd-4cca-b648-a437be61c5cd"]
    .Request()
    .Select("allowExternalSenders,autoSubscribeNewMembers,isSubscribedByMail,unseenCount")
    .GetAsync();

```