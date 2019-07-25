---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 43d2c079e547a5c704f587601cb2273c66884cb7
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35864485"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IChatMessageCollectionPage replies = graphClient.teams("303d2c1c-f1c5-40ce-b68e-544343d7f42b").channels("19:fec4b0f2825d4c8c82abc09027a64184@thread.skype").messages("1555375673184").replies()
    .buildRequest()
    .get();

```