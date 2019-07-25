---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 3a1738e96eb89120cd33cb01ba928a70a4eeec5a
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35876751"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IRoomListCollectionPage microsoft.graph.roomlist = graphClient.places().microsoft.graph.roomlist()
    .buildRequest()
    .get();

```