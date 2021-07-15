---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bffa957c56ddba9cf1af44eb0ff11d2ed484efbf
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53439136"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessPackageResourceRequest accessPackageResourceRequest = new AccessPackageResourceRequest();
accessPackageResourceRequest.catalogId = "beedadfe-01d5-4025-910b-84abb9369997";
accessPackageResourceRequest.requestType = "AdminAdd";
AccessPackageResource accessPackageResource = new AccessPackageResource();
accessPackageResource.originId = "c6294667-7348-4f5a-be73-9d2c65f574f3";
accessPackageResource.originSystem = "AadGroup";
accessPackageResourceRequest.accessPackageResource = accessPackageResource;

graphClient.identityGovernance().entitlementManagement().accessPackageResourceRequests()
    .buildRequest()
    .post(accessPackageResourceRequest);

```