---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 350b9a2f1d397dabac58ff9443b41919e9bc2a8cf6db86e0a22af218485ec9d4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902752"
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