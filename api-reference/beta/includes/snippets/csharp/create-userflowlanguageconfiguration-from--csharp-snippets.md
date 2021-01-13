---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 134be9770832bc2ca0824d9aa7031a9a03e297d9
ms.sourcegitcommit: a9731e19589dcb5c0c6fe2e24b008c86573ef803
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/13/2021
ms.locfileid: "49843901"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var userFlowLanguageConfiguration = new UserFlowLanguageConfiguration
{
    IsEnabled = false
};

await graphClient.Identity.B2cUserFlows["B2C_1_CustomerSignUp"].Languages["es-ES"]
    .Request()
    .PutAsync(userFlowLanguageConfiguration);

```