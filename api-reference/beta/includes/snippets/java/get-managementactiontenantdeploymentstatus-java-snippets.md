---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6366d59ba5aca14703dc9e1f22c88a5c1aaa04485f0b343cf263b797f6f6a74a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278072"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ManagementActionTenantDeploymentStatus managementActionTenantDeploymentStatus = graphClient.tenantRelationships().managedTenants().managementActionTenantDeploymentStatuses("{managementActionTenantDeploymentStatusId}")
    .buildRequest()
    .get();

```