---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 2d86ecdd7958137c531000a53d372035c3f5d6ce
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35892930"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String id = "id-value";

String groupId = "groupId-value";

graphClient.me().onenote().pages("{id}")
    .copyToSection(id,groupId,siteCollectionId,siteId)
    .buildRequest()
    .post();

```