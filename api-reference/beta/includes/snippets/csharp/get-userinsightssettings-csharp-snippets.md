---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a9f081a3bcf1191c50a90d44ca53319e60ffd8a5
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53210341"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var userInsightsSettings = await graphClient.Me.Settings.ItemInsights
    .Request()
    .GetAsync();

```