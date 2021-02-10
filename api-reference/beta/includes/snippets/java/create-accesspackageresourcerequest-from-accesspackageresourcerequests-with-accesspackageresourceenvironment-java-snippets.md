---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d06ff98ecd1c197d32bc916a065f5ec4add6a610
ms.sourcegitcommit: 48fff935d56fe96e97577a80a3a0aa15c45419ba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/10/2021
ms.locfileid: "50176331"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

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