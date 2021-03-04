---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 81f023a90752ddb86ed56affa415ef07acd4e27a
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50447695"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrinterCapabilities printerCapabilities = graphClient.print().printers("{id}")
    .getCapabilities()
    .buildRequest()
    .get();

```