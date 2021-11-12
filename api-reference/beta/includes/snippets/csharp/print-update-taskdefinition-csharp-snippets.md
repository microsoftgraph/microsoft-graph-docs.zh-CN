---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9b5d82ff884c9743b87e18ab63ffcdc2b8189c22e725910ef91c2c31aad29331
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332873"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var printTaskDefinition = new PrintTaskDefinition
{
    DisplayName = "Test TaskDefinitionName",
    CreatedBy = new AppIdentity
    {
        DisplayName = "Requesting App Display Name"
    }
};

await graphClient.Print.TaskDefinitions["{printTaskDefinition-id}"]
    .Request()
    .UpdateAsync(printTaskDefinition);

```