---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6198cec79b12083fe3a55f368bf1e94a290c050194d6d8ea335e3cc345c9b886
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158642"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessPackageResourceCollectionPage accessPackageResources = graphClient.identityGovernance().entitlementManagement().accessPackageCatalogs("{id}").accessPackageResources()
    .buildRequest()
    .filter("resourceType eq 'Application'")
    .expand("accessPackageResourceScopes")
    .get();

```