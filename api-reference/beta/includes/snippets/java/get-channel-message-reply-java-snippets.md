---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0dc8741576b04ad1ddccf3b5eead917e831a13b5
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50978791"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ChatMessage chatMessage = graphClient.teams("303d2c1c-f1c5-40ce-b68e-544343d7f42b").channels("19:fec4b0f2825d4c8c82abc09027a64184@thread.skype").messages("1555375673184").replies("1555377090002")
    .buildRequest()
    .get();

```