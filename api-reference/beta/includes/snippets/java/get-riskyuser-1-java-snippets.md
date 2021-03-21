---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 09a1f9e0bdac7dbb60c97e0d580b4e9f5de3c716
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50960769"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

RiskyUser riskyUser = graphClient.riskyUsers("c2b6c2b9-dddc-acd0-2b39-d519d803dbc3")
    .buildRequest()
    .get();

```