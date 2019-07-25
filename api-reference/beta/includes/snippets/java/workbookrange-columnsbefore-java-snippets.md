---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 3e42c685f7d469987916dd2bd10adf009f95bd90
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35866319"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.drive().root().workbook().worksheets("{id}")
    .range()
    .columnsBefore(count)
    .buildRequest()
    .post();

```