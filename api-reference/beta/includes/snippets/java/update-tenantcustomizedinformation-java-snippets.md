---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 70602247570c7149e998853c8ff77f75a30450fc77c7f9c48658be3c122014a3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333336"
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