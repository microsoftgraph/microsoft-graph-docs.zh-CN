---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3c23df603f18197f85ce86ce861e8b5eab0c5767
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50802974"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AppRoleAssignment appRoleAssignment = new AppRoleAssignment();
appRoleAssignment.principalId = UUID.fromString("cde330e5-2150-4c11-9c5b-14bfdc948c79");
appRoleAssignment.resourceId = UUID.fromString("8e881353-1735-45af-af21-ee1344582a4d");
appRoleAssignment.appRoleId = UUID.fromString("00000000-0000-0000-0000-000000000000");

graphClient.users("cde330e5-2150-4c11-9c5b-14bfdc948c79").appRoleAssignments()
    .buildRequest()
    .post(appRoleAssignment);

```