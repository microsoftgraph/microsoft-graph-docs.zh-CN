---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3d34d022d7363bf91356beb87620433c7554796b
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48981117"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IUnifiedRoleAssignmentCollectionPage roleAssignments = graphClient.roleManagement().directory().roleAssignments()
    .buildRequest()
    .filter(" principalId eq 'f1847572-48aa-47aa-96a3-2ec61904f41f'")
    .get();

```