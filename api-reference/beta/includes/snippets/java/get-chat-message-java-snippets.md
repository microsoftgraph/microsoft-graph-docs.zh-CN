---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d6b41904a40851044f52bc1f2e1fd968fbfe95f5
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48958309"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Chat chat = graphClient.users("{id}").chats("{id}")
    .buildRequest()
    .get();

```