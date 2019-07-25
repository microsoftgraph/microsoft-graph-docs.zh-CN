---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 6d9dca012eb07f7f0301aedf42f8fa2378eda869
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35863427"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ChatMessageHostedContent chatMessageHostedContent = graphClient.chats("{id}").messages("{id}").hostedContents("{id}")
    .buildRequest()
    .get();

```