---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 190f0afd17789d4a034f57846db9ad9d46181506
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35882224"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookChart workbookChart = graphClient.me().drive().items("{id}").workbook().worksheets("{id|name}").charts("{name}")
    .buildRequest()
    .get();

```