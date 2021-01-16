---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 14ea745423350d8f84883ff1e007eb1b1b7b3e84
ms.sourcegitcommit: 1d2adc4062c8e83d23768682cf66a731bccd313c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/16/2021
ms.locfileid: "49882880"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookRange workbookRange = graphClient.drive().root().workbook().worksheets("{id}")
    .range()
    .columnsAfter(2)
    .buildRequest()
    .get();

```