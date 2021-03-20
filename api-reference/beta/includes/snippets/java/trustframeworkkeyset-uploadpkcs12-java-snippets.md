---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 96aaa066c9f456772b51162b442f98d60596802d
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50978356"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String key = "Base64-encoded-pfx-content";

String password = "password-value";

graphClient.trustFramework().keySets("{id}")
    .uploadPkcs12(TrustFrameworkKeySetUploadPkcs12ParameterSet
        .newBuilder()
        .withKey(key)
        .withPassword(password)
        .build())
    .buildRequest()
    .post();

```