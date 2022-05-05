---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f55f21cc36d52dd1505174fae68332daf6042f47
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65203788"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessPackageAssignmentAdditionalAccessCollectionPage additionalAccess = graphClient.identityGovernance().entitlementManagement().accessPackageAssignments()
    .additionalAccess(AccessPackageAssignmentAdditionalAccessParameterSet
        .newBuilder()
        .withAccessPackageId("2506aef1-3929-4d24-a61e-7c8b83d95e6f")
        .withIncompatibleAccessPackageId("d5d99728-8c0b-4ede-83d2-cf9b0e8dabfb")
        .build())
    .buildRequest()
    .expand("target")
    .get();

```