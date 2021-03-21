---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e7d7710ba0b197e65698bac2e2c1399a80f0c00e
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50983509"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Boolean disableUserAccounts = true;

graphClient.domains("{id}")
    .forceDelete(DomainForceDeleteParameterSet
        .newBuilder()
        .withDisableUserAccounts(disableUserAccounts)
        .build())
    .buildRequest()
    .post();

```