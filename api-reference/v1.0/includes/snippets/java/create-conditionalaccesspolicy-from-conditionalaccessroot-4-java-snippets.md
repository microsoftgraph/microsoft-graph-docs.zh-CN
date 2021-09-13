---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a075bf3668a65e2b3324f70f73a1092465e310ab6b66c23f8a1c2cf2c39fd48d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333994"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ConditionalAccessPolicy conditionalAccessPolicy = new ConditionalAccessPolicy();
conditionalAccessPolicy.displayName = "Require MFA to EXO from non-compliant devices.";
conditionalAccessPolicy.state = ConditionalAccessPolicyState.ENABLED;
ConditionalAccessConditionSet conditions = new ConditionalAccessConditionSet();
ConditionalAccessApplications applications = new ConditionalAccessApplications();
LinkedList<String> includeApplicationsList = new LinkedList<String>();
includeApplicationsList.add("00000002-0000-0ff1-ce00-000000000000");
applications.includeApplications = includeApplicationsList;
conditions.applications = applications;
ConditionalAccessUsers users = new ConditionalAccessUsers();
LinkedList<String> includeGroupsList = new LinkedList<String>();
includeGroupsList.add("ba8e7ded-8b0f-4836-ba06-8ff1ecc5c8ba");
users.includeGroups = includeGroupsList;
conditions.users = users;
conditionalAccessPolicy.conditions = conditions;
ConditionalAccessGrantControls grantControls = new ConditionalAccessGrantControls();
grantControls.operator = "OR";
LinkedList<ConditionalAccessGrantControl> builtInControlsList = new LinkedList<ConditionalAccessGrantControl>();
builtInControlsList.add(ConditionalAccessGrantControl.MFA);
grantControls.builtInControls = builtInControlsList;
conditionalAccessPolicy.grantControls = grantControls;

graphClient.identity().conditionalAccess().policies()
    .buildRequest()
    .post(conditionalAccessPolicy);

```