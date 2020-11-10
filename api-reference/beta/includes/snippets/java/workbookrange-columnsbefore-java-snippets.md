---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7f8e38ae911c26b25406e0ab587f9612f38aa1d1
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48975921"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.drive().root().workbook().worksheets("{id}")
    .range()
    .columnsBefore(null)
    .buildRequest()
    .post();

```