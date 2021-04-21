---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 889d65e3c8569345ef432bc0e36578e06067a497
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/21/2021
ms.locfileid: "51921464"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IdentityProviderBase identityProviderBase = graphClient.identity().identityProviders("Amazon-OAUTH")
    .buildRequest()
    .get();

```