---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1267a29d7fbbeb61a4bde2eabcfd44c8655feeb0
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/16/2020
ms.locfileid: "49692602"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Case _case = new Case();
_case.displayName = "My Case 1 - Renamed";
_case.description = "Updated description";
_case.externalId = "Updated externalId";

graphClient.compliance().ediscovery().cases("061b9a92-8926-4bd9-b41d-abf35edc7583")
    .buildRequest()
    .patch(_case);

```