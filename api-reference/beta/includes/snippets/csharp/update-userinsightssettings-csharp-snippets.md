---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6c829ddeb2537031842487a0c4aba41cbc05a09b
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53210660"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var userInsightsSettings = new UserInsightsSettings
{
    IsEnabled = false
};

await graphClient.Users["{user-id}"].Settings.ItemInsights
    .Request()
    .UpdateAsync(userInsightsSettings);

```