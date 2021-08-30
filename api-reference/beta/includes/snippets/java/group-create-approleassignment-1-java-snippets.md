---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9614f43ecf3291b122be617c76ae5b87f04456d335b96a80dd3baa2c7a583f07
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104391"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AppRoleAssignment appRoleAssignment = new AppRoleAssignment();
appRoleAssignment.principalId = UUID.fromString("7679d9a4-2323-44cd-b5c2-673ec88d8b12");
appRoleAssignment.resourceId = UUID.fromString("076e8b57-bac8-49d7-9396-e3449b685055");
appRoleAssignment.appRoleId = UUID.fromString("00000000-0000-0000-0000-000000000000");

graphClient.groups("7679d9a4-2323-44cd-b5c2-673ec88d8b12").appRoleAssignments()
    .buildRequest()
    .post(appRoleAssignment);

```