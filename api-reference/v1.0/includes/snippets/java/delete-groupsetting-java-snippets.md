---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 74f81a3bab6ad7aa2f68c451c001a81a476289f7
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35886791"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.groupSettings("{id}")
    .buildRequest()
    .delete();

```