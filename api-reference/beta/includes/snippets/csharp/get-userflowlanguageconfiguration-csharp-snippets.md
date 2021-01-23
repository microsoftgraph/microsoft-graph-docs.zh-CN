---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 90abe87926ed52a027adf938f20c4f8cfbb7fdfa
ms.sourcegitcommit: 9a5facff47a8d4e05ecd2c6cd68294a948c47c4d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2021
ms.locfileid: "49944843"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var languages = await graphClient.Identity.B2cUserFlows["B2C_1_CustomerSignUp"].Languages
    .Request()
    .GetAsync();

```