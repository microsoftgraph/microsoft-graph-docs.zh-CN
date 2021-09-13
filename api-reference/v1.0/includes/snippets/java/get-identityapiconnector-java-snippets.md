---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2411f5a70078a969af5e721b50008bf2e1861224c1a78c7e82955950d0fd2afa
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163271"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IdentityApiConnector identityApiConnector = graphClient.identity().apiConnectors("370eeb68-dfd3-4a47-8160-8824c2358321")
    .buildRequest()
    .get();

```