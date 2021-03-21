---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d30864055640e953561a2f06c901361f3cc39e73
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50966940"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookPivotTable workbookPivotTable = graphClient.me().drive().root().workbook().worksheets("{id}").pivotTables("{id}")
    .buildRequest()
    .get();

```