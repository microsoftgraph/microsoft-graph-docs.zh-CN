---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 344e2d477da9ce327fe6a4311d5fbf31a92199708345738baef090d58ed3b982
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218546"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ConversationThread conversationThread = graphClient.groups("02bd9fd6-8f93-4758-87c3-1fb73740a315").threads("AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgMkABAAG5c7eC4NYEynIoXsuxXB9RAAG5c7eC4NYEynIoXsuxXB9Q==")
    .buildRequest()
    .get();

```