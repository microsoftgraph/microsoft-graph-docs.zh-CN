---
description: 自动生成的文件。 不修改
ms.openlocfilehash: eda27a5fbca725dd4a33430e94ff2a2698ea9edf
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35859449"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String comment = "comment-value";

boolean sendResponse = True;

graphClient.me().events("{id}")
    .tentativelyAccept(comment,sendResponse)
    .buildRequest()
    .post();

```