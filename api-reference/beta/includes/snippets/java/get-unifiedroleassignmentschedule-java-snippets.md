---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f6755778215179510f3b005711e0ee743420208b776cc3baa52c9c2c7acec7d1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274121"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UnifiedRoleAssignmentSchedule unifiedRoleAssignmentSchedule = graphClient.roleManagement().directory().roleAssignmentSchedules("b1477448-2cc6-4ceb-93b4-54a202a89413")
    .buildRequest()
    .get();

```