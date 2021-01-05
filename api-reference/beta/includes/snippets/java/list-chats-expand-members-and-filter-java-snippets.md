---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cfc2659a9d053689cf92c437fb35698704a3015f
ms.sourcegitcommit: a1675c7b8dfc7d7c3c7923d06cda2b0127f9c3e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/05/2021
ms.locfileid: "49752891"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IChatCollectionPage chats = graphClient.users("8b081ef6-4792-4def-b2c9-c363a1bf41d5").chats()
    .buildRequest()
    .filter("members/any(o: o/displayname eq 'Peter Parker')")
    .expand("members")
    .get();

```