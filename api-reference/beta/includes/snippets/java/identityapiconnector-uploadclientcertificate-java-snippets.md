---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ec7ac3f781784f784a39004549c9ace7a64e7e98
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/21/2021
ms.locfileid: "51920073"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String pkcs12Value = "eyJhbGciOiJSU0EtT0FFUCIsImVuYyI6IkEyNTZHQ00ifQ...kDJ04sJShkkgjL9Bm49plA";

String password = "<password>";

graphClient.identity().apiConnectors("{id}")
    .uploadClientCertificate(IdentityApiConnectorUploadClientCertificateParameterSet
        .newBuilder()
        .withPkcs12Value(pkcs12Value)
        .withPassword(password)
        .build())
    .buildRequest()
    .post();

```