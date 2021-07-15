---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dc0d11dcfe332532302aa74aebb5a72e6f25b8ed
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53439140"
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