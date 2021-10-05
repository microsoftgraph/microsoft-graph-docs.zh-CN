---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4d2fcc69da7468b20c83181d3f8a243b76dc5df37ee5dea4bbac376e24cf785f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274190"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ContinuousAccessEvaluationPolicy continuousAccessEvaluationPolicy = new ContinuousAccessEvaluationPolicy();
LinkedList<String> usersList = new LinkedList<String>();
usersList.add("88139f01-1f8d-4c06-ad74-a2544cee9aee");
continuousAccessEvaluationPolicy.users = usersList;
LinkedList<String> groupsList = new LinkedList<String>();
groupsList.add("9972fb3f-7a40-49f5-85f6-129d9dfbd47a");
groupsList.add("ea178055-4713-4d9a-a06c-ff17466b7e77");
continuousAccessEvaluationPolicy.groups = groupsList;

graphClient.identity().continuousAccessEvaluationPolicy()
    .buildRequest()
    .patch(continuousAccessEvaluationPolicy);

```