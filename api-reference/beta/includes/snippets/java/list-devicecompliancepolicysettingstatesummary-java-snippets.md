---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2f25ad5066526493dff909b7146bb271e26740da
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62137125"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DeviceCompliancePolicySettingStateSummaryCollectionPage deviceCompliancePolicySettingStateSummaries = graphClient.tenantRelationships().managedTenants().deviceCompliancePolicySettingStateSummaries()
    .buildRequest()
    .get();

```