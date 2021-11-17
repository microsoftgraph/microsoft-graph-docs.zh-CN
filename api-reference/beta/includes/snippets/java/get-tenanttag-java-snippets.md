---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a649eb9894aa5f4aa39fe8bdfd76536c2f4c47e5cebbaa99c184c995ce0e5267
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163137"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TenantTag tenantTag = graphClient.tenantRelationships().managedTenants().tenantTags("{tenantTagId}")
    .buildRequest()
    .get();

```