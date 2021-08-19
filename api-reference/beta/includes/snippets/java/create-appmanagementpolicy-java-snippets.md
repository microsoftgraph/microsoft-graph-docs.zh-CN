---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b35ff81b9bac68140cad9f858e2113ad2ea46ca2
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58262387"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AppManagementPolicy appManagementPolicy = new AppManagementPolicy();
appManagementPolicy.displayName = "Credential management policy";
appManagementPolicy.description = "Cred policy sample";
appManagementPolicy.isEnabled = true;
AppManagementConfiguration restrictions = new AppManagementConfiguration();
LinkedList<PasswordCredentialConfiguration> passwordCredentialsList = new LinkedList<PasswordCredentialConfiguration>();
PasswordCredentialConfiguration passwordCredentials = new PasswordCredentialConfiguration();
passwordCredentials.restrictionType = AppCredentialRestrictionType.PASSWORD_ADDITION;
passwordCredentials.maxLifetime = DatatypeFactory.newInstance().newDuration("null");
passwordCredentials.restrictForAppsCreatedAfterDateTime = OffsetDateTimeSerializer.deserialize("2019-10-19T10:37:00Z");
passwordCredentialsList.add(passwordCredentials);
PasswordCredentialConfiguration passwordCredentials1 = new PasswordCredentialConfiguration();
passwordCredentials1.restrictionType = AppCredentialRestrictionType.PASSWORD_LIFETIME;
passwordCredentials1.maxLifetime = DatatypeFactory.newInstance().newDuration("P4DT12H30M5S");
passwordCredentials1.restrictForAppsCreatedAfterDateTime = OffsetDateTimeSerializer.deserialize("2018-10-19T10:37:00Z");
passwordCredentialsList.add(passwordCredentials1);
restrictions.passwordCredentials = passwordCredentialsList;
appManagementPolicy.restrictions = restrictions;

graphClient.policies().appManagementPolicies()
    .buildRequest()
    .post(appManagementPolicy);

```