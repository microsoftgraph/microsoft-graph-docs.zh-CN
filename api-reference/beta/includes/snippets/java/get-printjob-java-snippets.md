---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6376301727a0a9626c889b1764fe8bd6bdd2a824
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50982719"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrintJob printJob = graphClient.print().printers("c05f3726-0d4b-4aa1-8fe9-2eb981bb26fb").jobs("5182")
    .buildRequest()
    .get();

```