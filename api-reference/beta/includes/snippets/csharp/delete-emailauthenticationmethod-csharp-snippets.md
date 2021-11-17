---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 49bd2eaa74465cfdf6708a54a4bb6b03cea8cb11d05a4cd95f443be6d5d6cdbd
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218943"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Users["{user-id}"].Authentication.EmailMethods["{emailAuthenticationMethod-id}"]
    .Request()
    .DeleteAsync();

```