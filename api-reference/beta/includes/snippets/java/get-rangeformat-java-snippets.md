---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a3fa85c64c77a25d7833e5ffa53d8e1e8f20afc4
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48973662"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookRangeFormat workbookRangeFormat = graphClient.me().drive().items("{id}").workbook().names("{name}")
    .range().format()
    .buildRequest()
    .get();

```