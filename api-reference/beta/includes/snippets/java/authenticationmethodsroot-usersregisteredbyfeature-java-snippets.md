---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 27126cf782f043adce3b1fd50c6787724d3bc49d
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50971630"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UserRegistrationFeatureSummary userRegistrationFeatureSummary = graphClient.reports().authenticationMethods()
    .usersRegisteredByFeature(AuthenticationMethodsRootUsersRegisteredByFeatureParameterSet
        .newBuilder()
        .withIncludedUserTypes('all')
        .withIncludedUserRoles('all')
        .build())
    .buildRequest()
    .get();

```