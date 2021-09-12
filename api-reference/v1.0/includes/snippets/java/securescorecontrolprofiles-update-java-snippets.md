---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6d2b8c2e1fae3b95dfba0418d75ed147576186330ec909775c806c449ce325b5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57409008"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SecureScoreControlProfile secureScoreControlProfile = new SecureScoreControlProfile();
secureScoreControlProfile.assignedTo = "";
secureScoreControlProfile.comment = "control is reviewed";
secureScoreControlProfile.state = "Reviewed";
SecurityVendorInformation vendorInformation = new SecurityVendorInformation();
vendorInformation.provider = "SecureScore";
vendorInformation.providerVersion = null;
vendorInformation.subProvider = null;
vendorInformation.vendor = "Microsoft";
secureScoreControlProfile.vendorInformation = vendorInformation;

graphClient.security().secureScoreControlProfiles("NonOwnerAccess")
    .buildRequest()
    .patch(secureScoreControlProfile);

```