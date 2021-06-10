---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5dacead2fa12380e83c7a3b7a5cbbf04e2fe5ddf
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2021
ms.locfileid: "52869127"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var roleDefinitions = await graphClient.RoleManagement.CloudPC.RoleDefinitions
    .Request()
    .GetAsync();

```