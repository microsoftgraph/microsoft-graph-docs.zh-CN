---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dd00b422caf0e3562551d528c8f1caf4f4d3488c
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2021
ms.locfileid: "52870344"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var unifiedRoleDefinition = await graphClient.RoleManagement.CloudPC.RoleDefinitions["{unifiedRoleDefinition-id}"]
    .Request()
    .GetAsync();

```