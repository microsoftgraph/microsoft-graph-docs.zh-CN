---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d392742de37070d1ce7517c2a753779fa9ea08ea
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50978763"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessPackageResourceRequest accessPackageResourceRequest = new AccessPackageResourceRequest();
accessPackageResourceRequest.catalogId = "26ac0c0a-08bc-4a7b-a313-839f58044ba5";
accessPackageResourceRequest.requestType = "AdminAdd";
accessPackageResourceRequest.justification = "";
AccessPackageResource accessPackageResource = new AccessPackageResource();
accessPackageResource.displayName = "Sales";
accessPackageResource.description = "https://contoso.sharepoint.com/sites/Sales";
accessPackageResource.url = "https://contoso.sharepoint.com/sites/Sales";
accessPackageResource.resourceType = "SharePoint Online Site";
accessPackageResource.originId = "https://contoso.sharepoint.com/sites/Sales";
accessPackageResource.originSystem = "SharePointOnline";
accessPackageResourceRequest.accessPackageResource = accessPackageResource;

graphClient.identityGovernance().entitlementManagement().accessPackageResourceRequests()
    .buildRequest()
    .post(accessPackageResourceRequest);

```