---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 90b190edf991284993742a97f0f3b3ee967c6d70
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50968061"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IdentityApiConnector identityApiConnector = new IdentityApiConnector();
identityApiConnector.displayName = "Test API";
identityApiConnector.targetUrl = "https://someapi.com/api";
BasicAuthentication authenticationConfiguration = new BasicAuthentication();
authenticationConfiguration.username = "<USERNAME>";
authenticationConfiguration.password = "<PASSWORD>";
identityApiConnector.authenticationConfiguration = authenticationConfiguration;

graphClient.identity().apiConnectors()
    .buildRequest()
    .post(identityApiConnector);

```