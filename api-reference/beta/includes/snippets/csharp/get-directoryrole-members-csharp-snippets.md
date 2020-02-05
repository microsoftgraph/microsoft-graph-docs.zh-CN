---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1901c9d5e421c768fa1b46b1f584398324daeb99
ms.sourcegitcommit: 7b286637aa332cfd534a41526950b4f6272e0fd7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/05/2020
ms.locfileid: "41774279"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var members = await graphClient.DirectoryRoles["{id}"].Members
    .Request()
    .GetAsync();

```