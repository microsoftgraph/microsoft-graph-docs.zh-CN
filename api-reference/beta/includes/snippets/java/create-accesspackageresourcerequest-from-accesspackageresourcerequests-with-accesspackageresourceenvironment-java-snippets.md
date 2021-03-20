---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f3858f769d528cf12292f804dce6e7e215bea13c
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50968405"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessPackageResourceRequest accessPackageResourceRequest = new AccessPackageResourceRequest();
accessPackageResourceRequest.catalogId = "de9315c1-272b-4905-924b-cc112ca180c7";
AccessPackageResource accessPackageResource = new AccessPackageResource();
accessPackageResource.displayName = "Community Outreach";
accessPackageResource.description = "https://contoso.sharepoint.com/sites/CSR";
accessPackageResource.resourceType = "SharePoint Online Site";
accessPackageResource.originId = "https://contoso.sharepoint.com/sites/CSR";
accessPackageResource.originSystem = "SharePointOnline";
accessPackageResource.additionalDataManager().put("accessPackageResourceEnvironment@odata.bind", new JsonPrimitive("accessPackageResourceEnvironments/615f2218-678f-471f-a60a-02c2f4f80c57"));
accessPackageResourceRequest.accessPackageResource = accessPackageResource;
accessPackageResourceRequest.requestType = "AdminAdd";

graphClient.identityGovernance().entitlementManagement().accessPackageResourceRequests()
    .buildRequest()
    .post(accessPackageResourceRequest);

```