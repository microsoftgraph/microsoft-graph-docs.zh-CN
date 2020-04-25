---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 30c3297bd9223525e139b2c9df3acbb2bb959b71
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43806253"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ActivityBasedTimeoutPolicy activityBasedTimeoutPolicy = new ActivityBasedTimeoutPolicy();
LinkedList<String> definitionList = new LinkedList<String>();
definitionList.add("definition-value");
activityBasedTimeoutPolicy.definition = definitionList;
activityBasedTimeoutPolicy.displayName = "displayName-value";
activityBasedTimeoutPolicy.isOrganizationDefault = true;
activityBasedTimeoutPolicy.type = "type-value";

graphClient.policies().activityBasedTimeoutPolicies("{id}")
    .buildRequest()
    .patch(activityBasedTimeoutPolicy);

```