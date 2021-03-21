---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6ab9bb417ef1cfab46d6c41b05101d9aa33958d1
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50967286"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrivilegedRoleAssignment privilegedRoleAssignment = graphClient.privilegedRoleAssignments("{id}")
    .buildRequest()
    .get();

```