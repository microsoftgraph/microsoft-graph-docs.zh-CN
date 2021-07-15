---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2ab4ef8bf3f43870d8e082918755c52a509ef95d
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53439912"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

GroupCollectionPage incompatibleGroups = graphClient.identityGovernance().entitlementManagement().accessPackages("{id}").incompatibleGroups()
    .buildRequest()
    .get();

```