---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ab88d98c06126bef0bcd4819e349dc7470ecbf01
ms.sourcegitcommit: 726f20403323be7d267b67c2764ed7c244e02ee1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/02/2020
ms.locfileid: "47330270"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.TermStore.Groups["{groupId}"]
    .Request()
    .DeleteAsync();

```