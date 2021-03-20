---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3856678f51d967084eaaef68b8faffa5c0307aee
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50978910"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessPackageResourceRoleCollectionPage accessPackageResourceRoles = graphClient.identityGovernance().entitlementManagement().accessPackageCatalogs("15d889df-3eb8-4e9b-bfb4-b1908849aec4").accessPackageResourceRoles()
    .buildRequest()
    .filter("(originSystem eq 'AadGroup' and accessPackageResource/id eq 'a35bef72-a8aa-4ca3-af30-f6b2ece7208f')")
    .expand("accessPackageResource/id%20eq%20'a35bef72-a8aa-4ca3-af30-f6b2ece7208f')")
    .get();

```