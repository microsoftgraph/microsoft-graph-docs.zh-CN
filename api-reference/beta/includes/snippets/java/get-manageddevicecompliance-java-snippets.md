---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e3c2c8f05f1120073605627cfa0a518a22a2a9d3474b0cce6cb15ae02cd3ef8e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57329028"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ManagedDeviceCompliance managedDeviceCompliance = graphClient.tenantRelationships().managedTenants().managedDeviceCompliances("{managedDeviceComplianceId}")
    .buildRequest()
    .get();

```