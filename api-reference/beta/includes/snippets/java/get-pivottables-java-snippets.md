---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 17215c990458a6d8983384daedfe410439b5ca41
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35866283"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IWorkbookPivotTableCollectionPage pivotTables = graphClient.drive().root().workbook().worksheets("{id}").pivotTables()
    .buildRequest()
    .get();

```