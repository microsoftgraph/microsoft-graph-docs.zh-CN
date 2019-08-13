---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 680000b25fdf2ef77d15b09f7e4104edf51ceda2
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36307783"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookRangeView workbookRangeView = graphClient.me().drive().root().workbook().worksheets("{id}")
    .range("A1:Z10")
    .visibleView()
    .buildRequest()
    .get();

```