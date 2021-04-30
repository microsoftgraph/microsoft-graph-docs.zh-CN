---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 20adb7553932638f1e82c9ae75a7fdb42e5a035c
ms.sourcegitcommit: e440d855f1106390d842905d97ceb16f143db2e5
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/29/2021
ms.locfileid: "52080591"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Chat chat = graphClient.chats("19:b8577894a63548969c5c92bb9c80c5e1@thread.v2")
    .buildRequest()
    .expand("members")
    .get();

```