---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3aefe9e7b0b373684f83ff8d2c38f9f7fa72539a
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53439198"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessPackageCollectionWithReferencesPage accessPackagesIncompatibleWith = graphClient.identityGovernance().entitlementManagement().accessPackages("{id}").accessPackagesIncompatibleWith()
    .buildRequest()
    .get();

```