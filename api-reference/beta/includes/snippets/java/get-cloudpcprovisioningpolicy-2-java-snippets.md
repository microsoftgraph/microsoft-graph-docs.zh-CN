---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 62d4eb2052539fad0e1972fd1e398ecc04a5f2471dffac9acb3dea78a65b6e18
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219264"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

CloudPcProvisioningPolicy cloudPcProvisioningPolicy = graphClient.deviceManagement().virtualEndpoint().provisioningPolicies("{id}")
    .buildRequest()
    .expand("assignments")
    .get();

```