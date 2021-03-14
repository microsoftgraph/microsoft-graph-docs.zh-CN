---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 31e991b3902eec642280f295d14b48e7c822409d
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50783379"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IAppRoleAssignmentCollectionPage appRoleAssignments = graphClient.servicePrincipals("8e881353-1735-45af-af21-ee1344582a4d").appRoleAssignments()
    .buildRequest()
    .get();

```