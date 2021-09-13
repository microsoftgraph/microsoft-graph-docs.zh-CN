---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7d7801d72d91fab94270e23556f800c3af82c2f408431816cf7f7c95948a6932
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279653"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var subscription = await graphClient.Me.Drive.Root.Subscriptions["{subscription-id}"]
    .Request()
    .GetAsync();

```