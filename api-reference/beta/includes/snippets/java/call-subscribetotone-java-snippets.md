---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 6eb0effb655e8130e01889d06904b49f2a1f6c81
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35864615"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String clientContext = "d45324c1-fcb5-430a-902c-f20af696537c";

graphClient.app().calls("{id}")
    .subscribeToTone(clientContext)
    .buildRequest()
    .post();

```