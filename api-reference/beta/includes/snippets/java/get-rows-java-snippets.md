---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b2db7fb2a71eab7573b1e30cef5b5c7430185484
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48975681"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IWorkbookRangeViewCollectionPage rows = graphClient.drive().root().workbook().worksheets("{id}")
    .range("A1:Z10")
    .visibleView().rows()
    .buildRequest()
    .get();

```