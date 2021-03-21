---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5357577f9fb2843bff663cd42980415eacb9a550
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50972510"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ConversationMemberCollectionPage members = graphClient.teams("2ab9c796-2902-45f8-b712-7c5a63cf41c4").channels("19:20bc1df46b1148e9b22539b83bc66809@thread.skype").members()
    .buildRequest()
    .get();

```