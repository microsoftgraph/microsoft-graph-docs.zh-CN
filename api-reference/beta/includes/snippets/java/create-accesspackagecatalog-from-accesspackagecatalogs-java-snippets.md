---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2619c64c1db6a74427b6bcf0a6339bf43958def3
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50971834"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessPackageCatalog accessPackageCatalog = new AccessPackageCatalog();
accessPackageCatalog.displayName = "sales";
accessPackageCatalog.description = "for employees working with sales and outside sales partners";
accessPackageCatalog.isExternallyVisible = true;

graphClient.identityGovernance().entitlementManagement().accessPackageCatalogs()
    .buildRequest()
    .post(accessPackageCatalog);

```