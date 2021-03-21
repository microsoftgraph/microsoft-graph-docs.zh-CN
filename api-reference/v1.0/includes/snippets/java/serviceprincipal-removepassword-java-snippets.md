---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 00717ed24872c8e721ff4a31fa3efaf9de496e78
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50972446"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UUID keyId = UUID.fromString("f0b0b335-1d71-4883-8f98-567911bfdca6");

graphClient.servicePrincipals("{id}")
    .removePassword(ServicePrincipalRemovePasswordParameterSet
        .newBuilder()
        .withKeyId(keyId)
        .build())
    .buildRequest()
    .post();

```