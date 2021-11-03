---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c7fd0b39b8fc09e60c889ef1092d0995e03967c8
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60718044"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ContinuousAccessEvaluationPolicy continuousAccessEvaluationPolicy = new ContinuousAccessEvaluationPolicy();
continuousAccessEvaluationPolicy.migrate = true;

graphClient.identity().continuousAccessEvaluationPolicy()
    .buildRequest()
    .patch(continuousAccessEvaluationPolicy);

```