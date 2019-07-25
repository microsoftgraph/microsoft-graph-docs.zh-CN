---
description: 自动生成的文件。 不修改
ms.openlocfilehash: ba07150a6be3c77e035afb26a176a31980293891
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35876945"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.users("{id|userPrincipalName}").photo()
    .buildRequest()
    .delete();

```