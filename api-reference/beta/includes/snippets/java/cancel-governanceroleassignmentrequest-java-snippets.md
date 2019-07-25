---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 42f5ee17744b2e7f3c9c0a86859e45efdc732967
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35859127"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.privilegedAccess("azureResources").roleAssignmentRequests("7c53453e-d5a4-41e0-8eb1-32d5ec8bfdee")
    .cancel()
    .buildRequest()
    .post();

```