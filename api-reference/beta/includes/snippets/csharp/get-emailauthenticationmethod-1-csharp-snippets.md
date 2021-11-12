---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8c8634dfdbf06e98625a26df61d832a707299232eb44b71f851070769c04e2f4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163234"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var emailAuthenticationMethod = await graphClient.Me.Authentication.EmailMethods["{emailAuthenticationMethod-id}"]
    .Request()
    .GetAsync();

```