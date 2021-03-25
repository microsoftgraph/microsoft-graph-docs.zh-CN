---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f4e08445ca494754c952e6b310da7e5efb2ba77d
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51208308"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ConditionalAccessPolicy conditionalAccessPolicy = new ConditionalAccessPolicy();
conditionalAccessPolicy.displayName = "Access to EXO requires MFA";
conditionalAccessPolicy.state = ConditionalAccessPolicyState.ENABLED;
ConditionalAccessConditionSet conditions = new ConditionalAccessConditionSet();
LinkedList<ConditionalAccessClientApp> clientAppTypesList = new LinkedList<ConditionalAccessClientApp>();
clientAppTypesList.add(ConditionalAccessClientApp.MOBILE_APPS_AND_DESKTOP_CLIENTS);
clientAppTypesList.add(ConditionalAccessClientApp.BROWSER);
conditions.clientAppTypes = clientAppTypesList;
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
ConditionalAccessLocations locations = new ConditionalAccessLocations();
LinkedList<String> includeLocationsList = new LinkedList<String>();
includeLocationsList.add("All");
locations.includeLocations = includeLocationsList;
LinkedList<String> excludeLocationsList = new LinkedList<String>();
excludeLocationsList.add("AllTrusted");
locations.excludeLocations = excludeLocationsList;
conditions.locations = locations;
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