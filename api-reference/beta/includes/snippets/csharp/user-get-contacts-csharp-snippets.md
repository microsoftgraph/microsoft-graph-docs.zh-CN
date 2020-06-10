---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 67997b6bb8559cd356917395b987d9880d07e965
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2020
ms.locfileid: "44684977"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var contacts = await graphClient.Me.Contacts
    .Request()
    .Select("displayName,emailAddresses")
    .GetAsync();

```