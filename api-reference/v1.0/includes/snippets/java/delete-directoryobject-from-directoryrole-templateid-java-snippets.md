---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 02e121d054900653c0f7a4477b70cb9ba844b2fa
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/01/2020
ms.locfileid: "49522796"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.directoryRoles("roleTemplateId={role-templateId}").members("{user-id}").reference()
    .buildRequest()
    .delete();

```