---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fdf0b4c946016cd1908477d646c564726cdedecb
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48978135"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IUnifiedRoleAssignmentMultipleCollectionPage roleAssignments = graphClient.roleManagement().deviceManagement().roleAssignments()
    .buildRequest()
    .filter(" principalIds/any(x:x eq '564ae70c-73d9-476b-820b-fb61eb7384b9')")
    .get();

```