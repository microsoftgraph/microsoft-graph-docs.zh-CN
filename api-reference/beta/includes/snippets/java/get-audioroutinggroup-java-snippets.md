---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 54e95cd0f189a9c69148d48f0b48ea17e796a86c
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35856911"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AudioRoutingGroup AudioRoutingGroup = graphClient.app().calls("{id}").audioRoutingGroups("{id}")
    .buildRequest()
    .get();

```