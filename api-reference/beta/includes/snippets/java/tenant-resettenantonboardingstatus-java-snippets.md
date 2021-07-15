---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d9a31b3e46ef3fec55772fe702f4a49c07713afd
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53440406"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.tenantRelationships().managedTenants().tenants("{tenantId}")
    .resetTenantOnboardingStatus()
    .buildRequest()
    .post();

```