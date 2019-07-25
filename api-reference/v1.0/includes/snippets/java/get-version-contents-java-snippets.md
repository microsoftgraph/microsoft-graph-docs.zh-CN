---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 95044bb2dc94268df612f544f1ee68bc6b9a36fc
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35857246"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Stream Stream = graphClient.customRequest("/me/drive/items/{item-id}/versions/{version-id}/content", Stream.class)
    .buildRequest()
    .get();

```