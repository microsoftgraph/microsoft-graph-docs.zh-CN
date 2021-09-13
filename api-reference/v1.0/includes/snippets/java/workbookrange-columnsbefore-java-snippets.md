---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d68d1ca1f57005c1ba4fd18cf89b387fe6fcb1a2408d5f4176e7e3be4c1a7455
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57164122"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookRange workbookRange = graphClient.me().drive().root().workbook().worksheets("{id}")
    .range()
    .columnsBefore(WorkbookRangeColumnsBeforeParameterSet
        .newBuilder()
        .withCount(2)
        .build())
    .buildRequest()
    .get();

```