---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 134213a713ec96a516a6d4958b0b7a37a070083452f3ecc5b503bd09c893dd95
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57103924"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String key = "key-value";

graphClient.trustFramework().keySets("{id}")
    .uploadCertificate(TrustFrameworkKeySetUploadCertificateParameterSet
        .newBuilder()
        .withKey(key)
        .build())
    .buildRequest()
    .post();

```