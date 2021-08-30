---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 69ddafcd6fedcdf601592565b6d5b6f6c25a77c55622f3efa757e50ae685fd97
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162741"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AppRoleAssignment appRoleAssignment = new AppRoleAssignment();
appRoleAssignment.principalId = UUID.fromString("9028d19c-26a9-4809-8e3f-20ff73e2d75e");
appRoleAssignment.resourceId = UUID.fromString("8fce32da-1246-437b-99cd-76d1d4677bd5");
appRoleAssignment.appRoleId = UUID.fromString("498476ce-e0fe-48b0-b801-37ba7e2685c6");

graphClient.servicePrincipals("9028d19c-26a9-4809-8e3f-20ff73e2d75e").appRoleAssignments()
    .buildRequest()
    .post(appRoleAssignment);

```