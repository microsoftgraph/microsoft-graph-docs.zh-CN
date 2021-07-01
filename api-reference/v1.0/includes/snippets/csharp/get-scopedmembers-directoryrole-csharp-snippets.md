---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2b730d71cfc828da73ee5afec043a22e9d74768e
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53208056"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var scopedMembers = await graphClient.DirectoryRoles["{directoryRole-id}"].ScopedMembers
    .Request()
    .GetAsync();

```