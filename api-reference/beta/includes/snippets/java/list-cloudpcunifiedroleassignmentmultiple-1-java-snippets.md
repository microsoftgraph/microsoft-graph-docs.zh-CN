---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 94e0143542fc7b459b6a6b27abf193ba6791038c4b159a3b9581e5ade8f2934b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278913"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UnifiedRoleAssignmentMultipleCollectionPage roleAssignments = graphClient.roleManagement().cloudPC().roleAssignments()
    .buildRequest()
    .get();

```