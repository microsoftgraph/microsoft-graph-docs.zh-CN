---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 480463dfd4793496c513e09ab310afa7482adea2
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2020
ms.locfileid: "44683886"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var delta = await graphClient.Users
    .Delta()
    .Request()
    .Select("displayName,jobTitle,mobilePhone")
    .GetAsync();

```