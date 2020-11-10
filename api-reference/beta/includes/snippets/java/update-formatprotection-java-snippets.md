---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 44638368147d4bd2ff055449578410151ab30a78
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48965508"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookFormatProtection workbookFormatProtection = new WorkbookFormatProtection();
workbookFormatProtection.locked = true;
workbookFormatProtection.formulaHidden = true;

graphClient.me().drive().items("{id}").workbook().names("{name}")
    .range().format().protection()
    .buildRequest()
    .patch(workbookFormatProtection);

```