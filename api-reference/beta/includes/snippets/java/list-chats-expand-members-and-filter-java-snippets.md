---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3609d2f07ce853be5bed0341afdc4f58a818f658
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50984078"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ChatCollectionPage chats = graphClient.users("8b081ef6-4792-4def-b2c9-c363a1bf41d5").chats()
    .buildRequest()
    .filter("members/any(o: o/displayname eq 'Peter Parker')")
    .expand("members")
    .get();

```