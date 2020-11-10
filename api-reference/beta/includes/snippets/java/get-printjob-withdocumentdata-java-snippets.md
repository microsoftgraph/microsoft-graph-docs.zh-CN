---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cf76fe2243735f2c417b6359cfa99287ae5b09a8
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48968337"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrintJob printJob = graphClient.print().printers("86b6d420-7e6b-4797-a05c-af4e56cd81bd").jobs("31216")
    .buildRequest()
    .expand("documents")
    .get();

```