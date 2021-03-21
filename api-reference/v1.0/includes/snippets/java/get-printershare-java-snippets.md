---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0016fcb2ffe8a725ca65c344e8b88877f76c02ba
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50983867"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrinterShare printerShare = graphClient.print().shares("{printerShareId}")
    .buildRequest()
    .get();

```