---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: de5cf32988d70feb6e0de369d9a0d81b150cac667239da7f553ded62c42c330c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902299"
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