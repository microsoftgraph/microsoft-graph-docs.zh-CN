---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 452a36dc95d2f8d467d2f5e4d5b068a8e3da9339
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50953121"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IRiskyUserHistoryItemCollectionPage history = graphClient.riskyUsers("41a31b00-3b3b-42d9-8f1c-6d4f14e74c69").history()
    .buildRequest()
    .get();

```