---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4d2a5924fdf17943ec208af12872a721173532ac
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53441521"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AggregatedPolicyComplianceCollectionPage aggregatedPolicyCompliances = graphClient.tenantRelationships().managedTenants().aggregatedPolicyCompliances()
    .buildRequest()
    .get();

```