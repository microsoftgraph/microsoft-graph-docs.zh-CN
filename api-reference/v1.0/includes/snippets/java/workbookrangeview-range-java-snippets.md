---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 1b2fa7819e6c5e16357125455e04cffd61b53eef
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35889673"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookRange workbookRange = graphClient.me().drive().root().workbook().worksheets("{id}")
    .range('A1:Z10')
    .visibleView()
    .range()
    .buildRequest()
    .get();

```