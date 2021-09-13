---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b6a130214fe153b740a19fd908ec14e0e2b47adccbbd6a56e663109b386d3384
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104612"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String entityType = "Group";

String displayName = "Myprefix_test_mysuffix";

String mailNickname = "Myprefix_test_mysuffix";

UUID onBehalfOfUserId = UUID.fromString("onBehalfOfUserId-value");

graphClient.directoryObjects()
    .validateProperties(DirectoryObjectValidatePropertiesParameterSet
        .newBuilder()
        .withEntityType(entityType)
        .withDisplayName(displayName)
        .withMailNickname(mailNickname)
        .withOnBehalfOfUserId(onBehalfOfUserId)
        .build())
    .buildRequest()
    .post();

```