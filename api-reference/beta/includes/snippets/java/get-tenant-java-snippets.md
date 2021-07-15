---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8868edc097cec5dcd3228bdc33842f8eeef6d0e8
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53442482"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Tenant tenant = graphClient.tenantRelationships().managedTenants().tenants("{tenantId}")
    .buildRequest()
    .get();

```