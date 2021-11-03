---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 369234082a2579d848232015efe304d92406d7f7
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60689216"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var federatedIdentityCredentials = await graphClient.Applications["{application-id}"].FederatedIdentityCredentials
    .Request()
    .GetAsync();

```