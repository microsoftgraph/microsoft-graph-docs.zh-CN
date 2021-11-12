---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d1f56aa9fe391040e62937f07b8ba1971a6a3a2f96dbde97776f5532cdefe7a3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57378388"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var subscriptions = await graphClient.Subscriptions
    .Request()
    .GetAsync();

```