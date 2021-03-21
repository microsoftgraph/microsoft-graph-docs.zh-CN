---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0e9bad52820d17c1f9ede0e20becef60c580692d
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50979994"
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