---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f1cadb932d6b7b824da41f496a5dce200a59453c
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/21/2020
ms.locfileid: "44334207"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.servicePrincipals("{id}").appRoleAssignments("{id}")
    .buildRequest()
    .delete();

```