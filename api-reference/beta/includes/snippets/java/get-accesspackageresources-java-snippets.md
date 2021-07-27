---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8ed07ff1cb4be803cd0ea8e4a4d43323862d1daf
ms.sourcegitcommit: 5bb981b4853663354a566d4a4a5cbf288939e441
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/24/2021
ms.locfileid: "53581189"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessPackageResourceCollectionPage accessPackageResources = graphClient.identityGovernance().entitlementManagement().accessPackageCatalogs("{id}").accessPackageResources()
    .buildRequest()
    .filter("resourceType eq 'Application'")
    .expand("accessPackageResourceScopes")
    .get();

```