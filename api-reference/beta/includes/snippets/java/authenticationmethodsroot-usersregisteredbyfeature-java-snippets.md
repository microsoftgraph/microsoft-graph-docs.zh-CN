---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9d7b5139cf5147f5d1589fd08e175b91c140ab1b244a2646ff124ccc21c9f73f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105060"
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