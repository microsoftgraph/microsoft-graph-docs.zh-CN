---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 6f81d1ce49df0222c7c2dea35f05ed306a414a9f
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35884976"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().drive().root().workbook().worksheets("{id}")
    .range()
    .rowsAbove(count)
    .buildRequest()
    .post();

```