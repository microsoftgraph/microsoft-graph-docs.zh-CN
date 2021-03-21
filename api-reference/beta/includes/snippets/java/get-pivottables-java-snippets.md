---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 51f6778f4259540c65cc8d3188298a13a5ad9acd
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50977714"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookPivotTableCollectionPage pivotTables = graphClient.drive().root().workbook().worksheets("{id}").pivotTables()
    .buildRequest()
    .get();

```