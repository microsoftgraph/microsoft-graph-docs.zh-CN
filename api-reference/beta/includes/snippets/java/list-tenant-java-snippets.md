---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f1ea0f5b097e594637f8d1ca7a26490d7fc7d592
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53440788"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TenantCollectionPage tenants = graphClient.tenantRelationships().managedTenants().tenants()
    .buildRequest()
    .get();

```