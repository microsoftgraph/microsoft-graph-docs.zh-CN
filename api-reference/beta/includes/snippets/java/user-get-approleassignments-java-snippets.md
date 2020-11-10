---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 39caca82d7b0a56e8e8ca4603697d196fb6f4469
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48977162"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IAppRoleAssignmentCollectionPage appRoleAssignments = graphClient.users("{id}").appRoleAssignments()
    .buildRequest()
    .get();

```