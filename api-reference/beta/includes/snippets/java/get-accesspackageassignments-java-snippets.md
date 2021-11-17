---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b98ef65a40d765bc799922e610bf94c20296d90e3b78cc506f01f329a9d29593
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902822"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessPackageAssignmentCollectionPage accessPackageAssignments = graphClient.identityGovernance().entitlementManagement().accessPackageAssignments()
    .buildRequest()
    .get();

```