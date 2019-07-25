---
description: 自动生成的文件。 不修改
ms.openlocfilehash: a79abf2ef51df33aef024a1d5ac159d34a382ee3
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35890819"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IGroupDeltaCollectionPage delta = graphClient.groups()
    .delta()
    .buildRequest()
    .select("displayName,description,mailNickname")
    .get();

```