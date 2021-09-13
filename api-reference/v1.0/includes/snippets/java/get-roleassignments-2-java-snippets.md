---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d4e7660609fa8512735c5443148bfa37ac09a484
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59130417"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UnifiedRoleAssignmentCollectionPage roleAssignments = graphClient.roleManagement().directory().roleAssignments()
    .buildRequest()
    .filter(" principalId eq 'f1847572-48aa-47aa-96a3-2ec61904f41f'")
    .get();

```