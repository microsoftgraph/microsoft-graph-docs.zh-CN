---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 46feac4572d0a7fa38d68ed956ebc02db5a03b40
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48981962"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IPrivilegedRoleAssignmentMyCollectionPage my = graphClient.privilegedRoleAssignments()
    .my()
    .buildRequest()
    .get();

```