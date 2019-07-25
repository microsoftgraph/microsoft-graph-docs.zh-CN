---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 6262508001c3419c7b52326a375e836fae8f55d7
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35862321"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String entityType = "Group";

String displayName = "Myprefix_test_mysuffix";

String mailNickname = "Myprefix_test_mysuffix";

String onBehalfOfUserId = "onBehalfOfUserId-value";

graphClient.directoryObjects()
    .validateProperties(entityType,displayName,mailNickname,onBehalfOfUserId)
    .buildRequest()
    .post();

```