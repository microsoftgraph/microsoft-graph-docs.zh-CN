---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b867522a10714855180da6a8f7b17042d4b63e023dd1b4ae18eee349f70a15e8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104208"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessPackage accessPackage = new AccessPackage();
accessPackage.catalogId = "aa2f6514-3232-46e7-a08a-2411ad8d7128";
accessPackage.displayName = "sales reps";
accessPackage.description = "outside sales representatives";

graphClient.identityGovernance().entitlementManagement().accessPackages()
    .buildRequest()
    .post(accessPackage);

```