---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 00d4320292676ce7504d76a7b7fee65c8883c0c5e1b7e2f432aad1cb28d2f01a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57378595"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var temporaryAccessPassAuthenticationMethod = await graphClient.Users["{user-id}"].Authentication.TemporaryAccessPassMethods["{temporaryAccessPassAuthenticationMethod-id}"]
    .Request()
    .GetAsync();

```