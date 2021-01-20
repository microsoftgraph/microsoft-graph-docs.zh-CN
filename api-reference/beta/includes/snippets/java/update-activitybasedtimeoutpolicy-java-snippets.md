---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c78f56d93e45de8ea6f923664387d1e23e7eed16
ms.sourcegitcommit: 6314172db76ba9f2c192d8c099d818c5e772d2b8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2021
ms.locfileid: "49910573"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ActivityBasedTimeoutPolicy activityBasedTimeoutPolicy = new ActivityBasedTimeoutPolicy();
LinkedList<String> definitionList = new LinkedList<String>();
definitionList.add("definition-value");
activityBasedTimeoutPolicy.definition = definitionList;
activityBasedTimeoutPolicy.displayName = "displayName-value";
activityBasedTimeoutPolicy.isOrganizationDefault = true;

graphClient.policies().activityBasedTimeoutPolicies("{id}")
    .buildRequest()
    .patch(activityBasedTimeoutPolicy);

```