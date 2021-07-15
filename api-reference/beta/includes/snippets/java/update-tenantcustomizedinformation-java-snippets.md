---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d4ce8759d8fd756d6e64e5d7b2508b2e84459cbe
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53441802"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TenantCustomizedInformation tenantCustomizedInformation = new TenantCustomizedInformation();
tenantCustomizedInformation.tenantId = "String";
LinkedList<TenantContactInformation> contactsList = new LinkedList<TenantContactInformation>();
TenantContactInformation contacts = new TenantContactInformation();
contactsList.add(contacts);
tenantCustomizedInformation.contacts = contactsList;
tenantCustomizedInformation.website = "String";

graphClient.tenantRelationships().managedTenants().tenantsCustomizedInformation("{tenantCustomizedInformationId}")
    .buildRequest()
    .patch(tenantCustomizedInformation);

```