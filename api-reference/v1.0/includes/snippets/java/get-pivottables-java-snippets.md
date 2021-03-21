---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1f0c6fb9ad22ae5e869e4b913e687cffa7f7f7aa
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50979794"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookPivotTableCollectionPage pivotTables = graphClient.me().drive().root().workbook().worksheets("{id}").pivotTables()
    .buildRequest()
    .get();

```