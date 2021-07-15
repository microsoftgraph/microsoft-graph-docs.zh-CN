---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: eae02d8ae7d647a82fd1ef798f22d6a31dd38f95
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53439968"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Content response = graphClient.tenantRelationships().managedTenants().deviceCompliancePolicySettingStateSummarys().{deviceCompliancePolicySettingStateSummaryId}()
    .buildRequest()
    .get();

```