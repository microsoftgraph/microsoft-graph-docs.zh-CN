---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e86cea2dfb6d0cbf6a0d9c3486be108f28fdbb8afc455707b1030015a2530ee4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57409795"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var call = await graphClient.Communications.Calls["{call-id}"]
    .Request()
    .GetAsync();

```