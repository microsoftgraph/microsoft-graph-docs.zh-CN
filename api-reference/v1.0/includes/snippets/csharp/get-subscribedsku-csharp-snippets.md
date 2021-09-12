---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 260b39b058b178087621ffcce7a4e87b9c178ff037f58d016a472ab9b2f35f05
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220374"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var subscribedSku = await graphClient.SubscribedSkus["{subscribedSku-id}"]
    .Request()
    .GetAsync();

```