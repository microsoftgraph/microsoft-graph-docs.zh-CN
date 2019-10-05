---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 0fc6bfd588c90e3427331df475d9fd1c554e8fde
ms.sourcegitcommit: 46ee19b244349e2a1537f0c44c576d7c01cf03a9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/05/2019
ms.locfileid: "37402779"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String comment = "comment-value";

boolean sendResponse = true;

graphClient.me().events("{id}")
    .tentativelyAccept(sendResponse,comment)
    .buildRequest()
    .post();

```