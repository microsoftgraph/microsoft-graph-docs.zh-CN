---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 92b370ad659b82c8f216db1ad633cc4bf1ffb6b1
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53441612"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ManagedDeviceComplianceTrend managedDeviceComplianceTrend = graphClient.tenantRelationships().managedTenants().managedDeviceComplianceTrends("{managedDeviceComplianceTrendId}")
    .buildRequest()
    .get();

```