---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 24738d08b1cb13d4e8ca9477fb24a88899f437f4
ms.sourcegitcommit: 1d2adc4062c8e83d23768682cf66a731bccd313c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/16/2021
ms.locfileid: "49882943"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookRange workbookRange = graphClient.drive().root().workbook().worksheets("{id}")
    .range()
    .rowsAbove(2)
    .buildRequest()
    .get();

```