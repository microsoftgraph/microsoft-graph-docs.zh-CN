---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 87272af942b137bf1fbc59f1309f1908ec04c801ca84b9f60daa261dea85f9b9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106658"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Users["{user-id}"].Authentication.Fido2Methods["{fido2AuthenticationMethod-id}"]
    .Request()
    .DeleteAsync();

```