---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b7a4051617d77f840e8289b35b7333a56e133e53
ms.sourcegitcommit: a9731e19589dcb5c0c6fe2e24b008c86573ef803
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/13/2021
ms.locfileid: "49843614"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var userFlowLanguageConfiguration = await graphClient.Identity.B2cUserFlows["B2C_1_Customer"].Languages["en"]
    .Request()
    .GetAsync();

```