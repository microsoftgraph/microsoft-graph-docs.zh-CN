---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5832c76c519ca1e59ea4d61dc1dabcb866e57d27
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53442657"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ConditionalAccessPolicyCoverageCollectionPage conditionalAccessPolicyCoverages = graphClient.tenantRelationships().managedTenants().conditionalAccessPolicyCoverages()
    .buildRequest()
    .get();

```