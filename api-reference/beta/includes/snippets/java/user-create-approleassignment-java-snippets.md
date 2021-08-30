---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0691e176884a032d8aa6cd369441fcbe2faea75d9e0485bcb99c84ab629e7f4c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57378545"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AppRoleAssignment appRoleAssignment = new AppRoleAssignment();
appRoleAssignment.principalId = UUID.fromString("cde330e5-2150-4c11-9c5b-14bfdc948c79");
appRoleAssignment.resourceId = UUID.fromString("8e881353-1735-45af-af21-ee1344582a4d");
appRoleAssignment.appRoleId = UUID.fromString("00000000-0000-0000-0000-000000000000");

graphClient.users("cde330e5-2150-4c11-9c5b-14bfdc948c79").appRoleAssignments()
    .buildRequest()
    .post(appRoleAssignment);

```