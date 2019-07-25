---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 425f556e3297a8f0f65b0da3f4ee20c84367c57f
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35886879"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().drive().root().workbook().worksheets("{id}")
    .range()
    .columnsBefore(count)
    .buildRequest()
    .post();

```