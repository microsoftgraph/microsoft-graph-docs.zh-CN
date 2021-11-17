---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a96d5938d319e654052683646224a55562d0ae324219d6c7936e3444a9d37358
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902749"
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