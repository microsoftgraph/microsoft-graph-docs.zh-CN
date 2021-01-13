---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0fcdb10a58b609837fcec0ffad15c6849a0b206e
ms.sourcegitcommit: a9731e19589dcb5c0c6fe2e24b008c86573ef803
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/13/2021
ms.locfileid: "49844547"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

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