---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 33a8a8e4a1f90e05c7fa358c370aacc1b4ae33ee
ms.sourcegitcommit: 726f20403323be7d267b67c2764ed7c244e02ee1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/02/2020
ms.locfileid: "47330424"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.TermStore.Sets["{setId}"]
    .Request()
    .DeleteAsync();

```