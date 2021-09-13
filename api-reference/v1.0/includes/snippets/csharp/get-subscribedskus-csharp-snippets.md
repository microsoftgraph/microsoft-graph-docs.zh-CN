---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d17850d041c1bd187ccff747554e3b34ff135774879263c1d990b6d0589ac4f1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57409469"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var subscribedSkus = await graphClient.SubscribedSkus
    .Request()
    .GetAsync();

```