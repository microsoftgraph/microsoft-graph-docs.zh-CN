---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 51f1e3f88709ea30a315d771957009ee77cc4fd7
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50441045"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var me = await graphClient.Me
    .Request()
    .Select("Responsibilities")
    .GetAsync();

var responsibilities = me.Responsibilities;

```