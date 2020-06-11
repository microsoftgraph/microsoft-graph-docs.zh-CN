---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d8014fa97b12838370e9716c4efee1ca5e3089f6
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2020
ms.locfileid: "44684938"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var users = await graphClient.Users
    .Request()
    .Select("displayName,givenName,postalCode")
    .GetAsync();

```