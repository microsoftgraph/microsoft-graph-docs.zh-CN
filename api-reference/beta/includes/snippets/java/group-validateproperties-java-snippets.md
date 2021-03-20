---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3b3803e769296bb8caf95c431f92e9b46817e8f5
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50966946"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String displayName = "Myprefix_test_mysuffix";

String mailNickname = "Myprefix_test_mysuffix";

UUID onBehalfOfUserId = UUID.fromString("onBehalfOfUserId-value");

graphClient.groups("{id}")
    .validateProperties(GroupValidatePropertiesParameterSet
        .newBuilder()
        .withDisplayName(displayName)
        .withMailNickname(mailNickname)
        .withOnBehalfOfUserId(onBehalfOfUserId)
        .build())
    .buildRequest()
    .post();

```