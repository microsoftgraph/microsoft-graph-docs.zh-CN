---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 97f46774df10267d6dafdcc261b3e6b48a67a2842cf03234c8d0f6d3cf7dae9e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162485"
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