---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 4780eae5c6dcf43c6285e771aeb223009f6af23d
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35868440"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookTableSort workbookTableSort = graphClient.me().drive().items("{id}").workbook().tables("{id|name}").sort()
    .buildRequest()
    .get();

```