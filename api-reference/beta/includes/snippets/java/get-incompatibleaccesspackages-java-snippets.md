---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7144ef667e426e878cdcdcd440fba7b0bf9dbb31
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65203837"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessPackageCollectionWithReferencesPage incompatibleAccessPackages = graphClient.identityGovernance().entitlementManagement().accessPackages("{id}").incompatibleAccessPackages()
    .buildRequest()
    .get();

```