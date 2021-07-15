---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 129667ec552113868634b99ae821250f2c87d6b6
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53441313"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.servicePrincipals("{resource-SP-id}").appRoleAssignedTo("{appRoleAssignment-id}")
    .buildRequest()
    .delete();

```