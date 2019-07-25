---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 9cd24f18e521fb48888b489d4f6b9ad4b750adfe
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35866344"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.drive().root().workbook().worksheets("{id}")
    .range()
    .rowsBelow(count)
    .buildRequest()
    .post();

```