---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: df9fe199058f8361be3decd786829510abd51f11
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59130421"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var roleDefinitions = await graphClient.RoleManagement.Directory.RoleDefinitions
    .Request()
    .GetAsync();

```