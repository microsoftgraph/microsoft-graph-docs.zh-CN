---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a9cc652dfb8352024d20d24bbc9a123e32a0ff05
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50981396"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IdentityApiConnector identityApiConnector = new IdentityApiConnector();
identityApiConnector.displayName = "New Test API";
identityApiConnector.targetUrl = "https://otherapi.com/api/endpoint";
BasicAuthentication authenticationConfiguration = new BasicAuthentication();
authenticationConfiguration.username = "<NEW_USERNAME>";
authenticationConfiguration.password = "<NEW_PASSWORD>";
identityApiConnector.authenticationConfiguration = authenticationConfiguration;

graphClient.identity().apiConnectors("{identityApiConnectorId}")
    .buildRequest()
    .patch(identityApiConnector);

```