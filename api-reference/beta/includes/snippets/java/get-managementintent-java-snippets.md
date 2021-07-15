---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 91f879036468253a18f5f1c941fc2c1e15e76baf
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53442565"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ManagementIntent managementIntent = graphClient.tenantRelationships().managedTenants().managementIntents("{managementIntentId}")
    .buildRequest()
    .get();

```