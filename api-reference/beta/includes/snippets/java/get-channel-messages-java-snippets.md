---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 963d7ce60d8622c377504438e37777a2674eb3a3
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50978971"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ChatMessageCollectionPage messages = graphClient.teams("303d2c1c-f1c5-40ce-b68e-544343d7f42b").channels("19:fec4b0f2825d4c8c82abc09027a64184@thread.skype").messages()
    .buildRequest()
    .get();

```