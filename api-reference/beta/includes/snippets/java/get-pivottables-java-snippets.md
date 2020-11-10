---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 17215c990458a6d8983384daedfe410439b5ca41
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48970757"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IWorkbookPivotTableCollectionPage pivotTables = graphClient.drive().root().workbook().worksheets("{id}").pivotTables()
    .buildRequest()
    .get();

```