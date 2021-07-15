---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a79880eed3b20819df62bad98a58ebff79353f70
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53440312"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TenantCustomizedInformation tenantCustomizedInformation = graphClient.tenantRelationships().managedTenants().tenantsCustomizedInformation("{tenantCustomizedInformationId}")
    .buildRequest()
    .get();

```