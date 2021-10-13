---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d560de9e95612e2195314451939e9425cf2e74a2a825ba4b54d5382e3ac80598
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277770"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Oauth2PermissionGrants["{oAuth2PermissionGrant-id}"]
    .Request()
    .DeleteAsync();

```