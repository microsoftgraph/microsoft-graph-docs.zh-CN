---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 44002de245f949afcaef6d896626af94542c0078
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35875645"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IPrivilegedRoleAssignmentCollectionPage my = graphClient.privilegedRoleAssignments()
    .my()
    .buildRequest()
    .get();

```