---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8b5037cad711bae4d492cce6f4462b0c58455fc5
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60690104"
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
passwordCredentials1.restrictForAppsCreatedAfterDateTime = OffsetDateTimeSerializer.deserialize("2014-10-19T10:37:00Z");
passwordCredentialsList.add(passwordCredentials1);
PasswordCredentialConfiguration passwordCredentials2 = new PasswordCredentialConfiguration();
passwordCredentials2.restrictionType = AppCredentialRestrictionType.SYMMETRIC_KEY_ADDITION;
passwordCredentials2.maxLifetime = DatatypeFactory.newInstance().newDuration("null");
passwordCredentials2.restrictForAppsCreatedAfterDateTime = OffsetDateTimeSerializer.deserialize("2019-10-19T10:37:00Z");
passwordCredentialsList.add(passwordCredentials2);
PasswordCredentialConfiguration passwordCredentials3 = new PasswordCredentialConfiguration();
passwordCredentials3.restrictionType = AppCredentialRestrictionType.SYMMETRIC_KEY_LIFETIME;
passwordCredentials3.maxLifetime = DatatypeFactory.newInstance().newDuration("P4D");
passwordCredentials3.restrictForAppsCreatedAfterDateTime = OffsetDateTimeSerializer.deserialize("2014-10-19T10:37:00Z");
passwordCredentialsList.add(passwordCredentials3);
restrictions.passwordCredentials = passwordCredentialsList;
LinkedList<KeyCredentialConfiguration> keyCredentialsList = new LinkedList<KeyCredentialConfiguration>();
KeyCredentialConfiguration keyCredentials = new KeyCredentialConfiguration();
keyCredentials.restrictionType = AppKeyCredentialRestrictionType.ASYMMETRIC_KEY_LIFETIME;
keyCredentials.maxLifetime = DatatypeFactory.newInstance().newDuration("P90D");
keyCredentials.restrictForAppsCreatedAfterDateTime = OffsetDateTimeSerializer.deserialize("2014-10-19T10:37:00Z");
keyCredentialsList.add(keyCredentials);
restrictions.keyCredentials = keyCredentialsList;
appManagementPolicy.restrictions = restrictions;

graphClient.policies().appManagementPolicies()
    .buildRequest()
    .post(appManagementPolicy);

```