---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5099052f43abe4eabcb731a530d92f359f3700d4
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50978351"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

OnenoteSection onenoteSection = new OnenoteSection();
onenoteSection.displayName = "Section name";

graphClient.me().onenote().notebooks("{id}").sections()
    .buildRequest()
    .post(onenoteSection);

```