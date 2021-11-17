---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fcd1c6247393b4218adfc7564abf1fd63146bad30b1bc0d31b26713cb847d78a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902772"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessPackageResourceRoleCollectionPage accessPackageResourceRoles = graphClient.identityGovernance().entitlementManagement().accessPackageCatalogs("15d889df-3eb8-4e9b-bfb4-b1908849aec4").accessPackageResourceRoles()
    .buildRequest()
    .filter("(originSystem eq 'AadGroup' and accessPackageResource/id eq 'a35bef72-a8aa-4ca3-af30-f6b2ece7208f')")
    .expand("accessPackageResource/id%20eq%20'a35bef72-a8aa-4ca3-af30-f6b2ece7208f')")
    .get();

```