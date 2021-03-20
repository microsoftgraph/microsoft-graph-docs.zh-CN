---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5beb654e087fda6e07c4593a215451e75b119606
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50953125"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IRiskyUserHistoryItemCollectionPage history = graphClient.identityProtection().riskyUsers("41a31b00-3b3b-42d9-8f1c-6d4f14e74c69").history()
    .buildRequest()
    .get();

```