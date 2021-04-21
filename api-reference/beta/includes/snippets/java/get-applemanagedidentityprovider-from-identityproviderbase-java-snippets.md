---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b5bcb612aab58960642f4ee915b5f19ab515b7d8
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/21/2021
ms.locfileid: "51921461"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IdentityProviderBase identityProviderBase = graphClient.identity().identityProviders("Apple-Managed-OIDC")
    .buildRequest()
    .get();

```