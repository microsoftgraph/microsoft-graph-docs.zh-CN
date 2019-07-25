---
description: 自动生成的文件。 不修改
ms.openlocfilehash: f0e80a067a6ca55a55abab1360a5e8b33c9deb33
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35864764"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IAudioRoutingGroupCollectionPage audioRoutingGroups = graphClient.app().calls("{id}").audioRoutingGroups()
    .buildRequest()
    .get();

```