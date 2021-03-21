---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fbc8dbb3b6a93275307d11c5d9a49631619fea68
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50968887"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrinterShare printerShare = graphClient.print().shares("{printerShareId}")
    .buildRequest()
    .select("id,displayName,capabilities")
    .get();

```