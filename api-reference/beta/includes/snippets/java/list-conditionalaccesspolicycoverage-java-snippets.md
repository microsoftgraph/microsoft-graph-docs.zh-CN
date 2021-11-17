---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: efba0ec0391c28be7da0ff612911b3312d34cd25466627a60ae0edea33b419dc
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274160"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ConditionalAccessPolicyCoverageCollectionPage conditionalAccessPolicyCoverages = graphClient.tenantRelationships().managedTenants().conditionalAccessPolicyCoverages()
    .buildRequest()
    .get();

```