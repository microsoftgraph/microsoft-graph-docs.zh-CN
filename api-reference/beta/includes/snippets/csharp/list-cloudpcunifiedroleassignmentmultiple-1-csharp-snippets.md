---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 40b0cf296bbfe40bc5bde46b2ed527b5b52bc416
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2021
ms.locfileid: "52869010"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var roleAssignments = await graphClient.RoleManagement.CloudPC.RoleAssignments
    .Request()
    .GetAsync();

```