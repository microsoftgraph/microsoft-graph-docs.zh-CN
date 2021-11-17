---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6b7d89f406f7d447c634723bf3921e341b8dd8102dd6aa1238922ff633de5449
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56904218"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String displayName = "CN=customDisplayName";

OffsetDateTime endDateTime = OffsetDateTimeSerializer.deserialize("01/25/2024 00:00:00");

graphClient.servicePrincipals("004375c5-6e2e-4dec-95e3-626838cb9f80")
    .addTokenSigningCertificate(ServicePrincipalAddTokenSigningCertificateParameterSet
        .newBuilder()
        .withDisplayName(displayName)
        .withEndDateTime(endDateTime)
        .build())
    .buildRequest()
    .post();

```