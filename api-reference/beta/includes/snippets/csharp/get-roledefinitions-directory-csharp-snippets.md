---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: df9fe199058f8361be3decd786829510abd51f11
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2021
ms.locfileid: "52869128"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var roleDefinitions = await graphClient.RoleManagement.Directory.RoleDefinitions
    .Request()
    .GetAsync();

```