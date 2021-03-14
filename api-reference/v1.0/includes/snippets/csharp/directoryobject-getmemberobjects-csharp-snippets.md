---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3382cfc94e0876d714938363aed8db2372de6c95
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50810259"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var securityEnabledOnly = true;

await graphClient.DirectoryObjects["{directoryObject-id}"]
    .GetMemberObjects(securityEnabledOnly)
    .Request()
    .PostAsync();

```