---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 063918d41eb62b9606eeec9ab7aff85db425a6cd
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/21/2021
ms.locfileid: "51921230"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IdentityProviderBase identityProviderBase = new IdentityProviderBase();
identityProviderBase.clientSecret = "1111111111111";

graphClient.identity().identityProviders("Amazon-OAUTH")
    .buildRequest()
    .patch(identityProviderBase);

```