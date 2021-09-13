---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: eff09c65ec5ff5dbb59605f2ee62eeade3d777491e968f9fc31185bcd07cda55
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277834"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ConversationMember conversationMember = graphClient.teams("ece6f0a1-7ca4-498b-be79-edf6c8fc4d82").members("ZWUwZjVhZTItOGJjNi00YWU1LTg0NjYtN2RhZWViYmZhMDYyIyM3Mzc2MWYwNi0yYWM5LTQ2OWMtOWYxMC0yNzlhOGNjMjY3Zjk=")
    .buildRequest()
    .get();

```