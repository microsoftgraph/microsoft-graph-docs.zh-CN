---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 09f50ebede9122040e9f5a422b7f6d16759a7a7f
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53207955"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TeamsAsyncOperationCollectionPage operations = graphClient.chats("19:c253a29b5f694b55a6baad8e83510af7@thread.v2").operations()
    .buildRequest()
    .get();

```