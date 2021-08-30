---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a35c34160745e5012c837608900aeeb319a069884cae5d567a5a5167b73880f1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56904263"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ChannelGetAllMessagesCollectionPage getAllMessages = graphClient.teams("fbe2bf47-16c8-47cf-b4a5-4b9b187c508b").channels()
    .getAllMessages()
    .buildRequest()
    .get();

```