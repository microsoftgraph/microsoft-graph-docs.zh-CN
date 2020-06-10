---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3a030c54d54e38c82d4f13f29d6ae3c00b04e611
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2020
ms.locfileid: "44685028"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var delta = await graphClient.Contacts
    .Delta()
    .Request()
    .Select("displayName,jobTitle,mail")
    .GetAsync();

```