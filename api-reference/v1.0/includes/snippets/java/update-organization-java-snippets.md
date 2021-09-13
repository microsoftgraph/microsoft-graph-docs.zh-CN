---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5f4de5e2fb6b1e85e20fe603072041ba3c28a7d12102b0f820273f2c8c6b2f5c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332556"
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