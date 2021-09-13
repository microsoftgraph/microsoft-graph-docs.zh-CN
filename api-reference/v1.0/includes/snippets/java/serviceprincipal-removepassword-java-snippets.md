---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 392d10fa19b38a0163ac7c913537b6c01dbf275f17f3c72303940d94585a52e7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279323"
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