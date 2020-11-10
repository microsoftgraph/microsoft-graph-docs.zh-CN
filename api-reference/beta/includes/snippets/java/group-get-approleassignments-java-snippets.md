---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c9d9d7b94a791b931abe16654499ee935407e340
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48965166"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IAppRoleAssignmentCollectionPage appRoleAssignments = graphClient.groups("{id}").appRoleAssignments()
    .buildRequest()
    .get();

```