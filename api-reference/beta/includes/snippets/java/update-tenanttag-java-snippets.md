---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f17f260234006a39eb3d6bb547d13c5bb6ca550b8c29e397f7759b8a938ac97c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219173"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TenantTag tenantTag = new TenantTag();
tenantTag.displayName = "Onboarding";
tenantTag.description = "Tenants that we are currently onboarding";

graphClient.tenantRelationships().managedTenants().tenantTags("{tenantTagId}")
    .buildRequest()
    .patch(tenantTag);

```