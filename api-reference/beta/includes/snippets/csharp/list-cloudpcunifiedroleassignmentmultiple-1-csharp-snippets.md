---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c531cc0c52ce6ce04f49c26d32c07e1be902ee32efab29571ee392f7b5ed8ca1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57221221"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var roleAssignments = await graphClient.RoleManagement.CloudPC.RoleAssignments
    .Request()
    .GetAsync();

```