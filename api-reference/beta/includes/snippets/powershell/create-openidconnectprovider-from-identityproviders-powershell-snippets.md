---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 384af3f716a2e3104b541fe6ce224a43b80de19d
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62090027"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

$params = @{
    "@odata.type" = "microsoft.graph.openIdConnectProvider"
    Name = "Login with the Contoso identity provider"
    Type = "OpenIDConnect"
    ClientId = "56433757-cadd-4135-8431-2c9e3fd68ae8"
    ClientSecret = "12345"
    DomainHint = "mycustomoidc"
    MetadataUrl = "https://mycustomoidc.com/.well-known/openid-configuration"
    ResponseMode = "form_post"
    ResponseType = "code"
    Scope = "openid"
}

New-MgIdentityProvider -BodyParameter $params

```