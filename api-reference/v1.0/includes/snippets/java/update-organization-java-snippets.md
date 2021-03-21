---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c748a291fbc09140612a1fefa81da68ba4f88f04
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50980771"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Organization organization = new Organization();
LinkedList<String> marketingNotificationEmailsList = new LinkedList<String>();
marketingNotificationEmailsList.add("marketing@contoso.com");
organization.marketingNotificationEmails = marketingNotificationEmailsList;
PrivacyProfile privacyProfile = new PrivacyProfile();
privacyProfile.contactEmail = "alice@contoso.com";
privacyProfile.statementUrl = "https://contoso.com/privacyStatement";
organization.privacyProfile = privacyProfile;
LinkedList<String> securityComplianceNotificationMailsList = new LinkedList<String>();
securityComplianceNotificationMailsList.add("security@contoso.com");
organization.securityComplianceNotificationMails = securityComplianceNotificationMailsList;
LinkedList<String> securityComplianceNotificationPhonesList = new LinkedList<String>();
securityComplianceNotificationPhonesList.add("(123) 456-7890");
organization.securityComplianceNotificationPhones = securityComplianceNotificationPhonesList;
LinkedList<String> technicalNotificationMailsList = new LinkedList<String>();
technicalNotificationMailsList.add("tech@contoso.com");
organization.technicalNotificationMails = technicalNotificationMailsList;

graphClient.organization("{id}")
    .buildRequest()
    .patch(organization);

```