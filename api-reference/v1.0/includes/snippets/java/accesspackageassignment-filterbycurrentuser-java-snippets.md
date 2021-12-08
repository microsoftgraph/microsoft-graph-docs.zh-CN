---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7aaa7a32baec4d63078b12e58214e5bfa7a0dc89
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/08/2021
ms.locfileid: "61342884"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessPackageAssignmentFilterByCurrentUserCollectionPage filterByCurrentUser = graphClient.identityGovernance().entitlementManagement().assignments()
    .filterByCurrentUser(AccessPackageAssignmentFilterByCurrentUserParameterSet
        .newBuilder()
        .withOn('target')
        .build())
    .buildRequest()
    .get();

```