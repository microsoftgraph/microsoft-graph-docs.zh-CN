---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 62372979c023ab24c553efe70d69eb8b53216f62
ms.sourcegitcommit: a9731e19589dcb5c0c6fe2e24b008c86573ef803
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/13/2021
ms.locfileid: "49843964"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UserFlowApiConnectorConfiguration userFlowApiConnectorConfiguration = graphClient.customRequest("/identity/b2cUserFlows/B2C_1_testuserflow/apiConnectorConfiguration", UserFlowApiConnectorConfiguration.class)
    .buildRequest()
    .get();

```