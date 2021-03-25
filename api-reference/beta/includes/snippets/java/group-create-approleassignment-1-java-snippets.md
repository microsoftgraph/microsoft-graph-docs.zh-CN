---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2369129228df4e8e1c5d3431e9c8b769df5175f4
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51211048"
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