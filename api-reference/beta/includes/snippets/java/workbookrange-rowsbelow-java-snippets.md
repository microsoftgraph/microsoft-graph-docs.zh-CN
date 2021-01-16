---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6499e17ab9661ace414a025c92338c5783e9e7a2
ms.sourcegitcommit: 1d2adc4062c8e83d23768682cf66a731bccd313c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/16/2021
ms.locfileid: "49883082"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookRange workbookRange = graphClient.drive().root().workbook().worksheets("{id}")
    .range()
    .rowsBelow(2)
    .buildRequest()
    .get();

```