---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 955f1427f757ae73b5ae881e8f834882f8611d60
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53211909"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessPackageAssignmentRequestFilterByCurrentUserCollectionPage filterByCurrentUser = graphClient.identityGovernance().entitlementManagement().accessPackageAssignmentRequests()
    .filterByCurrentUser(AccessPackageAssignmentRequestFilterByCurrentUserParameterSet
        .newBuilder()
        .withOn('target')
        .build())
    .buildRequest()
    .get();

```