---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2252959231f6084cc0ac205d8ada4b07c914b1f6
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50976827"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

InputStream stream = graphClient.print().printers("fcb0bc53-a446-41d0-bfc3-5c56cdbb0f2a").jobs("46140").documents("bd260b1a-044e-4ca6-afa9-17d9a587d254").content()
    .buildRequest()
    .get();

```