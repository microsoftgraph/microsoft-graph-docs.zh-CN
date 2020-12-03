---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 14bdd637509892167f35d0f89eea49815a2ec94d
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/01/2020
ms.locfileid: "49523286"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IPermissionGrantConditionSetCollectionPage excludes = graphClient.policies().permissionGrantPolicies("microsoft-application-admin").excludes()
    .buildRequest()
    .get();

```