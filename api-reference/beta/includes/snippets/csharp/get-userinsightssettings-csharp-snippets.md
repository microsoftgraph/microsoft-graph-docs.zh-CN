---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c3eef05e6b809b7fbe53e9bcbda4cf3a5bf72bde49345c754ca406b1320d57c2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105949"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var userInsightsSettings = await graphClient.Me.Settings.ItemInsights
    .Request()
    .GetAsync();

```