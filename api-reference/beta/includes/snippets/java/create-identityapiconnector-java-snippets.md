---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: aaf8265d15ae0f60c44f73ce292e3552bf3cbd6a
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/21/2021
ms.locfileid: "51922599"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IdentityApiConnector identityApiConnector = new IdentityApiConnector();
identityApiConnector.displayName = "Test API";
identityApiConnector.targetUrl = "https://someotherapi.com/api";
Pkcs12Certificate authenticationConfiguration = new Pkcs12Certificate();
authenticationConfiguration.pkcs12Value = "eyJhbGciOiJSU0EtT0FFUCIsImVuYyI6IkEyNTZHQ00ifQ...kDJ04sJShkkgjL9Bm49plA";
authenticationConfiguration.password = "<password>";
identityApiConnector.authenticationConfiguration = authenticationConfiguration;

graphClient.identity().apiConnectors()
    .buildRequest()
    .post(identityApiConnector);

```