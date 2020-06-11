---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 48fa44fb125641be1883c9813728fa3600583e67
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2020
ms.locfileid: "44685026"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IRoomCollectionPage room = graphClient.places().microsoft.graph.room()
    .buildRequest()
    .get();

```