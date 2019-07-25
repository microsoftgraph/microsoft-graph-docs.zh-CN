---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 113534ab7abb68e8bbe4a4a2a223c76c6d78429a
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35862111"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.settings("{id}")
    .buildRequest()
    .delete();

```