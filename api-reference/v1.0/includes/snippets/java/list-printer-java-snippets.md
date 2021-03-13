---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 84c858cb5e4a9716b398b0db9cd9ca6aace66116
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50772399"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IPrinterCollectionPage printers = graphClient.print().printers()
    .buildRequest()
    .get();

```