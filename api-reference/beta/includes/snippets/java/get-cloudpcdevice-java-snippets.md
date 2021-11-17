---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3573553bab710945f418846131ca99c01b420fedcaa03282d17c3937dd8e4b3e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274162"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

CloudPcDevice cloudPcDevice = graphClient.tenantRelationships().managedTenants().cloudPcDevices("{cloudPcDeviceId}")
    .buildRequest()
    .get();

```