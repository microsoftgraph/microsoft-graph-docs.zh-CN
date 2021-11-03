---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4aa0747f4ddf4795f115cafeeb04015596a3da6781d13b6e5519f4907159e1f1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104189"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessPackageFilterByCurrentUserCollectionPage filterByCurrentUser = graphClient.identityGovernance().entitlementManagement().accessPackages()
    .filterByCurrentUser(AccessPackageFilterByCurrentUserParameterSet
        .newBuilder()
        .withOn('allowedRequestor')
        .build())
    .buildRequest()
    .get();

```