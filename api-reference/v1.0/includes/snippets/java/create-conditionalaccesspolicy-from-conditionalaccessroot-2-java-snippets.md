---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: da4d127187fa701cf636a7e17584202f4cb43870c235939d52c08c7605b8885c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279739"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ConditionalAccessPolicy conditionalAccessPolicy = new ConditionalAccessPolicy();
conditionalAccessPolicy.displayName = "Block access to EXO non-trusted regions.";
conditionalAccessPolicy.state = ConditionalAccessPolicyState.ENABLED;
ConditionalAccessConditionSet conditions = new ConditionalAccessConditionSet();
LinkedList<ConditionalAccessClientApp> clientAppTypesList = new LinkedList<ConditionalAccessClientApp>();
clientAppTypesList.add(ConditionalAccessClientApp.ALL);
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
includeLocationsList.add("198ad66e-87b3-4157-85a3-8a7b51794ee9");
locations.includeLocations = includeLocationsList;
conditions.locations = locations;
conditionalAccessPolicy.conditions = conditions;
ConditionalAccessGrantControls grantControls = new ConditionalAccessGrantControls();
grantControls.operator = "OR";
LinkedList<ConditionalAccessGrantControl> builtInControlsList = new LinkedList<ConditionalAccessGrantControl>();
builtInControlsList.add(ConditionalAccessGrantControl.BLOCK);
grantControls.builtInControls = builtInControlsList;
conditionalAccessPolicy.grantControls = grantControls;

graphClient.identity().conditionalAccess().policies()
    .buildRequest()
    .post(conditionalAccessPolicy);

```