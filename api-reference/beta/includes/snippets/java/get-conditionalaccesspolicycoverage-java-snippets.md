---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 311b2ddb1f37c9710475a907b79e0fecd96e6bbc
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53440114"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ConditionalAccessPolicyCoverage conditionalAccessPolicyCoverage = graphClient.tenantRelationships().managedTenants().conditionalAccessPolicyCoverages("{conditionalAccessPolicyCoverageId}")
    .buildRequest()
    .get();

```