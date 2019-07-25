---
description: 自动生成的文件。 不修改
ms.openlocfilehash: d0e3dfd431817d5d8114cb18f45a40db8ee8cf1a
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35883102"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookRangeFont workbookRangeFont = new WorkbookRangeFont();
workbookRangeFont.bold = true;
workbookRangeFont.color = "color-value";
workbookRangeFont.italic = true;
workbookRangeFont.name = "name-value";
workbookRangeFont.size = 99;
workbookRangeFont.underline = "underline-value";

graphClient.me().drive().items("{id}").workbook().names("{name}")
    .range().format().font()
    .buildRequest()
    .patch(workbookRangeFont);

```