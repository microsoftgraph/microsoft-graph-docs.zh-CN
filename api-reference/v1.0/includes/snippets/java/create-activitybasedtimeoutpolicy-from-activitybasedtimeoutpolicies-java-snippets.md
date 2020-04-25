---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 74b68eac61a2e2b21ada2e153db9fef7cfa1dffe
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43806328"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ActivityBasedTimeoutPolicy activityBasedTimeoutPolicy = new ActivityBasedTimeoutPolicy();
LinkedList<String> definitionList = new LinkedList<String>();
definitionList.add("definition-value");
activityBasedTimeoutPolicy.definition = definitionList;
activityBasedTimeoutPolicy.displayName = "displayName-value";
activityBasedTimeoutPolicy.isOrganizationDefault = true;

graphClient.policies().activityBasedTimeoutPolicies()
    .buildRequest()
    .post(activityBasedTimeoutPolicy);

```