---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 435a6214a1ac244acb9639b519c6bc3a9c913da8
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/08/2021
ms.locfileid: "61335483"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessPackageCatalog accessPackageCatalog = new AccessPackageCatalog();
accessPackageCatalog.displayName = "sales";
accessPackageCatalog.description = "for employees working with sales and outside sales partners";
accessPackageCatalog.state = AccessPackageCatalogState.PUBLISHED;
accessPackageCatalog.isExternallyVisible = true;

graphClient.identityGovernance().entitlementManagement().catalogs()
    .buildRequest()
    .post(accessPackageCatalog);

```