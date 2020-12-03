---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d7c0e7274534c953001460c0e5f81f558ee9441d
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/01/2020
ms.locfileid: "49521493"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.deviceManagement().virtualEndpoint().provisioningPolicies("{id}")
    .buildRequest()
    .delete();

```