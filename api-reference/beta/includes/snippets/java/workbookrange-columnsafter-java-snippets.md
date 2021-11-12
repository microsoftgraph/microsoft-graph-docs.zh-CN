---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c342284d283d044dda951264d4c09431357ce8f0099bdad58645e736a22dc18d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56904200"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookRange workbookRange = graphClient.drive().root().workbook().worksheets("{id}")
    .range()
    .columnsAfter(WorkbookRangeColumnsAfterParameterSet
        .newBuilder()
        .withCount(2)
        .build())
    .buildRequest()
    .get();

```