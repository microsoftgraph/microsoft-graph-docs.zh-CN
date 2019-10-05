---
description: 自动生成的文件。 不修改
ms.openlocfilehash: ac25ea6f4c643194270980784a2f8ff7ac41f1e1
ms.sourcegitcommit: 46ee19b244349e2a1537f0c44c576d7c01cf03a9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/05/2019
ms.locfileid: "37402856"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String comment = "comment-value";

boolean sendResponse = true;

graphClient.me().events("{id}")
    .accept(sendResponse,comment)
    .buildRequest()
    .post();

```