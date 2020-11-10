---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 188b8fbebfe937e2dd6fb0b3f1523c12d8b9006d
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48969588"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookPivotTable workbookPivotTable = graphClient.drive().root().workbook().worksheets("{id}").pivotTables("{id}")
    .buildRequest()
    .get();

```