---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 3b46fbc1aa948f0120e1f18bbf0cc13fa975e8b9
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35874490"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookRangeFont workbookRangeFont = graphClient.me().drive().items("{id}").workbook().names("{name}")
    .range().format().font()
    .buildRequest()
    .get();

```