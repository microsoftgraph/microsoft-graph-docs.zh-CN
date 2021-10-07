---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: da54c4bf63c960a6ff4669864f4be7c9f77722e4ab55dd4205e08952e1b0e7fd
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57328791"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Policies.AuthenticationMethodsPolicy.AuthenticationMethodConfigurations["{authenticationMethodConfiguration-id}"]
    .Request()
    .DeleteAsync();

```