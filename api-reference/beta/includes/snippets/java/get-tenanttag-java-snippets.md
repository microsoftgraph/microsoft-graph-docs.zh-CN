---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 37e2dff0d9b834f0b71bf9d4482288d2f3c6fd97
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53441075"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TenantTag tenantTag = graphClient.tenantRelationships().managedTenants().tenantTags("{tenantTagId}")
    .buildRequest()
    .get();

```