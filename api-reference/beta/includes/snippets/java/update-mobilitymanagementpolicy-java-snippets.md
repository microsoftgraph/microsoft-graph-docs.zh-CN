---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 13997875bf1ca21fcc6cc8798d5d01e7b48db469
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53440347"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

MobilityManagementPolicy mobilityManagementPolicy = new MobilityManagementPolicy();
mobilityManagementPolicy.complianceUrl = "https://portal.uem.contoso.com/?portalAction=Compliance";
mobilityManagementPolicy.discoveryUrl = "https://enrollment.uem.contoso.com/enrollmentserver/discovery.svc";
mobilityManagementPolicy.termsOfUseUrl = "https://portal.uem.contoso.com/TermsofUse.aspx";

graphClient.policies().mobileDeviceManagementPolicies("ab90bacf-55a3-4a3e-839a-aa4b74e4f020")
    .buildRequest()
    .patch(mobilityManagementPolicy);

```