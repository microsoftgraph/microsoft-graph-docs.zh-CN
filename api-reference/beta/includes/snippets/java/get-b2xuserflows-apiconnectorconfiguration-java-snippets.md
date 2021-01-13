---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5ad0fcd4ae548c9215dbd860c82f1e8c2c7ff13b
ms.sourcegitcommit: a9731e19589dcb5c0c6fe2e24b008c86573ef803
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/13/2021
ms.locfileid: "49843688"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UserFlowApiConnectorConfiguration userFlowApiConnectorConfiguration = graphClient.customRequest("/identity/b2xUserFlows/B2X_1_testuserflow/apiConnectorConfiguration", UserFlowApiConnectorConfiguration.class)
    .buildRequest()
    .get();

```