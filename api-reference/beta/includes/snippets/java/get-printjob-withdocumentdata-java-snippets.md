---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7fd3961833f55d3a510a78f53310e801ef525795
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50969960"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrintJob printJob = graphClient.print().printers("86b6d420-7e6b-4797-a05c-af4e56cd81bd").jobs("31216")
    .buildRequest()
    .expand("documents")
    .get();

```