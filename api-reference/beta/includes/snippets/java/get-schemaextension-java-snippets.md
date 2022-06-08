---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 99ed2ebe7bfa1f13079b2898413f996641903e17
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/08/2022
ms.locfileid: "65946798"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

User user = graphClient.users("4562bcc8-c436-4f95-b7c0-4f8ce89dca5e")
    .buildRequest()
    .select("ext55gb1l09_msLearnCourses")
    .get();

```