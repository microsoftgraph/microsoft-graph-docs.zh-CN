---
description: 自动生成的文件。 不修改
ms.openlocfilehash: dbc573230cb33dae87eedf6fd48c3a2a89578b75
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35859751"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String comment = "comment-value";

boolean sendResponse = True;

graphClient.me().events("{id}")
    .accept(comment,sendResponse)
    .buildRequest()
    .post();

```