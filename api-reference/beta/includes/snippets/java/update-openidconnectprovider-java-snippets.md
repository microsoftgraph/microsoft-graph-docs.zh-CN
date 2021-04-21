---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2c46732ee1b0b4795801b521661286207261bf22
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/21/2021
ms.locfileid: "51921217"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IdentityProviderBase identityProviderBase = new IdentityProviderBase();
identityProviderBase.responseType = EnumSet.of(OpenIdConnectResponseTypes.ID_TOKEN);

graphClient.identity().identityProviders("OIDC-V1-Nam_AD_Test-3e393390-ed2d-4794-97f6-5c999ccc61f7")
    .buildRequest()
    .patch(identityProviderBase);

```