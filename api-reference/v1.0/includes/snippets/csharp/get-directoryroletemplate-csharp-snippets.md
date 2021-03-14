---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a74a478ad7630a4607daf3c9007eb9bf7dcf9ee2
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50783951"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directoryRoleTemplate = await graphClient.DirectoryRoleTemplates["{directoryRoleTemplate-id}"]
    .Request()
    .GetAsync();

```