---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f46bdfd4f76bb3393eeb1a27d818d52b1e13541f
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50959061"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IUnifiedRoleAssignmentCollectionPage roleAssignments = graphClient.roleManagement().directory().roleAssignments()
    .buildRequest()
    .get();

```