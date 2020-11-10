---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c14e58e01811eb721e8b4a02a4106083465f92b8
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48979045"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookRangeView workbookRangeView = graphClient.drive().root().workbook().worksheets("{id}")
    .range("A1:Z10")
    .visibleView()
    .buildRequest()
    .get();

```