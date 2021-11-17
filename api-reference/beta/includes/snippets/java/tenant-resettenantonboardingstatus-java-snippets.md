---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9d783814ecc64d0f9ccec518e8d2b9db8e8278d38bdb5603bafb3d7ed8b8e45a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163397"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.tenantRelationships().managedTenants().tenants("{tenantId}")
    .resetTenantOnboardingStatus()
    .buildRequest()
    .post();

```