---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a8967450bcfaad46438f009206d0b8eaf1cd9de0f5d5c553f13dec48d5e5518d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105697"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var ownedObjects = await graphClient.Me.OwnedObjects
    .Request()
    .GetAsync();

```