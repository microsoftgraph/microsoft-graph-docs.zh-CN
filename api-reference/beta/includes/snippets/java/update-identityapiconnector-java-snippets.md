---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f1509059fc632d058f6a329695e2d4111c05a512
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/21/2021
ms.locfileid: "51922582"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IdentityApiConnector identityApiConnector = new IdentityApiConnector();
Pkcs12Certificate authenticationConfiguration = new Pkcs12Certificate();
authenticationConfiguration.pkcs12Value = "eyJhbGciOiJSU0EtT0FFUCIsImVuYyI6IkEyNTZHQ00ifQ...kDJ04sJShkkgjL9Bm49plA";
authenticationConfiguration.password = "secret";
identityApiConnector.authenticationConfiguration = authenticationConfiguration;

graphClient.identity().apiConnectors("{identityApiConnectorId}")
    .buildRequest()
    .patch(identityApiConnector);

```