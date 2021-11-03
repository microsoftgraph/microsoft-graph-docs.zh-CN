---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 57ceb62acbaa5fe6a1ca52fc40c3512a1dbf249e
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2021
ms.locfileid: "60676781"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TenantAppManagementPolicy tenantAppManagementPolicy = new TenantAppManagementPolicy();
tenantAppManagementPolicy.isEnabled = true;
AppManagementConfiguration applicationRestrictions = new AppManagementConfiguration();
LinkedList<PasswordCredentialConfiguration> passwordCredentialsList = new LinkedList<PasswordCredentialConfiguration>();
PasswordCredentialConfiguration passwordCredentials = new PasswordCredentialConfiguration();
passwordCredentials.restrictionType = AppCredentialRestrictionType.PASSWORD_ADDITION;
passwordCredentials.maxLifetime = DatatypeFactory.newInstance().newDuration("null");
passwordCredentials.restrictForAppsCreatedAfterDateTime = OffsetDateTimeSerializer.deserialize("2021-04-01T10:37:00Z");
passwordCredentialsList.add(passwordCredentials);
PasswordCredentialConfiguration passwordCredentials1 = new PasswordCredentialConfiguration();
passwordCredentials1.restrictionType = AppCredentialRestrictionType.PASSWORD_LIFETIME;
passwordCredentials1.maxLifetime = DatatypeFactory.newInstance().newDuration("P4DT12H30M5S");
passwordCredentials1.restrictForAppsCreatedAfterDateTime = OffsetDateTimeSerializer.deserialize("2019-01-01T10:37:00Z");
passwordCredentialsList.add(passwordCredentials1);
PasswordCredentialConfiguration passwordCredentials2 = new PasswordCredentialConfiguration();
passwordCredentials2.restrictionType = AppCredentialRestrictionType.SYMMETRIC_KEY_ADDITION;
passwordCredentials2.maxLifetime = DatatypeFactory.newInstance().newDuration("null");
passwordCredentials2.restrictForAppsCreatedAfterDateTime = OffsetDateTimeSerializer.deserialize("2021-04-01T10:37:00Z");
passwordCredentialsList.add(passwordCredentials2);
PasswordCredentialConfiguration passwordCredentials3 = new PasswordCredentialConfiguration();
passwordCredentials3.restrictionType = AppCredentialRestrictionType.SYMMETRIC_KEY_LIFETIME;
passwordCredentials3.maxLifetime = DatatypeFactory.newInstance().newDuration("P40D");
passwordCredentials3.restrictForAppsCreatedAfterDateTime = OffsetDateTimeSerializer.deserialize("2015-04-01T10:37:00Z");
passwordCredentialsList.add(passwordCredentials3);
applicationRestrictions.passwordCredentials = passwordCredentialsList;
LinkedList<KeyCredentialConfiguration> keyCredentialsList = new LinkedList<KeyCredentialConfiguration>();
KeyCredentialConfiguration keyCredentials = new KeyCredentialConfiguration();
keyCredentials.restrictionType = AppKeyCredentialRestrictionType.ASYMMETRIC_KEY_LIFETIME;
keyCredentials.maxLifetime = DatatypeFactory.newInstance().newDuration("P30D");
keyCredentials.restrictForAppsCreatedAfterDateTime = OffsetDateTimeSerializer.deserialize("2015-01-01T10:37:00Z");
keyCredentialsList.add(keyCredentials);
applicationRestrictions.keyCredentials = keyCredentialsList;
tenantAppManagementPolicy.applicationRestrictions = applicationRestrictions;

graphClient.policies().defaultAppManagementPolicy()
    .buildRequest()
    .patch(tenantAppManagementPolicy);

```