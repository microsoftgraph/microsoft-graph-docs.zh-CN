---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7e464cbcb7e24fdd173a6d43decc5582fb2819c3
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/05/2019
ms.locfileid: "37997464"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var webAccount = await graphClient.Me.Profile.WebAccounts["{id}"]
    .Request()
    .GetAsync();

```