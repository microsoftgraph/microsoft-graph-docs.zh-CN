---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6bda3ab69e89c5f00d25e0b99748b505e100513c
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2021
ms.locfileid: "52870666"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TimeCardCollectionPage timeCards = graphClient.teams("fd15cad8-80f6-484f-9666-3caf695fbf32").schedule().timeCards()
    .buildRequest()
    .filter("state eq 'clockedOut'")
    .top(2)
    .get();

```