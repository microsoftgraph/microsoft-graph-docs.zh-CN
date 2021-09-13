---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dfb33c17cd492e5ad6829559bb699adfb51b59384f26df12fa7a3f3aab0d4d52
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57409721"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AssignmentOrder assignmentOrder = graphClient.identity().b2xUserFlows("B2X_1_Partner").userAttributeAssignments()
    .getOrder()
    .buildRequest()
    .get();

```