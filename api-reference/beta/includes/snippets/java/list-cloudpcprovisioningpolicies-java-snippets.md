---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e6d5c97179d670cac161f1bee64c9c7a8910d3a3
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50977020"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

CloudPcProvisioningPolicyCollectionPage provisioningPolicies = graphClient.deviceManagement().virtualEndpoint().provisioningPolicies()
    .buildRequest()
    .get();

```