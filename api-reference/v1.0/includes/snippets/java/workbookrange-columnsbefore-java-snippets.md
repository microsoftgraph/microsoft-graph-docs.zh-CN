---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0a29e7067612b203aebe89fb835353f77cfd19a7
ms.sourcegitcommit: 1d2adc4062c8e83d23768682cf66a731bccd313c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/16/2021
ms.locfileid: "49883104"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookRange workbookRange = graphClient.me().drive().root().workbook().worksheets("{id}")
    .range()
    .columnsBefore(2)
    .buildRequest()
    .get();

```