---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 099494482ea58db28eaa0fb58820ccc3d28733d4
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65212875"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ConversationMemberCollectionWithReferencesPage allowedMembers = graphClient.teams("893075dd-2487-5634-925f-022c42e20265").channels("19:561fbdbbfca848a484f0a6f00ce9dbbd@thread.tacv2").sharedWithTeams("893075dd-2487-5634-925f-022c42e20265").allowedMembers()
    .buildRequest()
    .get();

```