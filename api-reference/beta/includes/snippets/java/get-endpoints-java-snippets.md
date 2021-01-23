---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4a23cfc22c4f18a6e4708974376d726ac60bbaf5
ms.sourcegitcommit: 9a5facff47a8d4e05ecd2c6cd68294a948c47c4d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2021
ms.locfileid: "49945359"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ReportRoot reportRoot = graphClient.print().reports("monthlyPrintUsageSummariesByPrinter")
    .buildRequest()
    .get();

```