---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dc09c3ea33e229167becab9593dd1d64c0bead49
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60695196"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var federatedIdentityCredential = await graphClient.Applications["{application-id}"].FederatedIdentityCredentials["{federatedIdentityCredential-id}"]
    .Request()
    .GetAsync();

```