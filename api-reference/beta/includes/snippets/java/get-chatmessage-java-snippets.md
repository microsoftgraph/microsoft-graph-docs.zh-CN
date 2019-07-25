---
description: 自动生成的文件。 不修改
ms.openlocfilehash: ddb37bbd59a0160ea75c8691cf2424ec60fdfb43
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35895383"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ChatMessage chatMessage = graphClient.chats("{id}").messages("{id}")
    .buildRequest()
    .get();

```