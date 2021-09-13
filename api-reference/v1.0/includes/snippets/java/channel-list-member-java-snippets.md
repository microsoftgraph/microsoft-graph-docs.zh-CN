---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 98b9ae7488c0d035d93bcedd4b36da1238b58734a9d19b8a64f4389be55cdcba
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903001"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ConversationMemberCollectionPage members = graphClient.teams("2ab9c796-2902-45f8-b712-7c5a63cf41c4").channels("19:20bc1df46b1148e9b22539b83bc66809@thread.skype").members()
    .buildRequest()
    .get();

```