---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 720386ffbc57369ac482d4d3fb5f618b4aa42cfd
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50777431"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IAppRoleAssignmentCollectionPage appRoleAssignments = graphClient.users("cdb555e3-b33e-4fd5-a427-17fadacbdfa7").appRoleAssignments()
    .buildRequest()
    .get();

```