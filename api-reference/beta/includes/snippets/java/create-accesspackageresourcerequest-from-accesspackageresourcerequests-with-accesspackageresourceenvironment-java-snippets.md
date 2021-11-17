---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2a6a2610f75c9e7984f612b3e05cfbd02203ff0451dfb223160ef25236e945fc
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902751"
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