---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b30b82234053a4dedf3336303217a98013b15c2c
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48970778"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookRange workbookRange = graphClient.drive().root().workbook().worksheets("{id}")
    .range("A1:Z10")
    .visibleView()
    .range()
    .buildRequest()
    .get();

```