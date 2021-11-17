---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 97d4ae74871bb3cae13c77f57546839ee93f580524846d818e14ee7208d839fc
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902750"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessPackageResourceRequest accessPackageResourceRequest = new AccessPackageResourceRequest();
accessPackageResourceRequest.catalogId = "beedadfe-01d5-4025-910b-84abb9369997";
accessPackageResourceRequest.requestType = "AdminRemove";
AccessPackageResource accessPackageResource = new AccessPackageResource();
accessPackageResource.id = "354078e5-dbce-4894-8af4-0ab274d41662";
accessPackageResourceRequest.accessPackageResource = accessPackageResource;

graphClient.identityGovernance().entitlementManagement().accessPackageResourceRequests()
    .buildRequest()
    .post(accessPackageResourceRequest);

```