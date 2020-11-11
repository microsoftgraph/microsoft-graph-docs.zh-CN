---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e44c423418f6792cc8df7c3eeeec75d625a9bca1
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48983306"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String entityType = "Group";

String displayName = "Myprefix_test_mysuffix";

String mailNickname = "Myprefix_test_mysuffix";

UUID onBehalfOfUserId = UUID.fromString("onBehalfOfUserId-value");

graphClient.directoryObjects()
    .validateProperties(entityType,displayName,mailNickname,onBehalfOfUserId)
    .buildRequest()
    .post();

```