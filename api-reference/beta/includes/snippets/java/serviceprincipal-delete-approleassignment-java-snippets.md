---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f1cadb932d6b7b824da41f496a5dce200a59453c
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48974184"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.servicePrincipals("{id}").appRoleAssignments("{id}")
    .buildRequest()
    .delete();

```