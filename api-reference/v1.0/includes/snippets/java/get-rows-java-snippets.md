---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 428d93629c32611e405894743fd8304849fbb95e
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35889700"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IWorkbookRangeViewCollectionPage rows = graphClient.me().drive().root().workbook().worksheets("{id}")
    .range('A1:Z10')
    .visibleView().rows()
    .buildRequest()
    .get();

```