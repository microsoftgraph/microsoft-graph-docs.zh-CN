---
description: 自动生成的文件。 不修改
ms.openlocfilehash: ac2996708d72716cac362470d95bd5c012cbe4fe
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35866374"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.drive().root().workbook().worksheets("{id}").pivotTables()
    .refreshAll()
    .buildRequest()
    .post();

```