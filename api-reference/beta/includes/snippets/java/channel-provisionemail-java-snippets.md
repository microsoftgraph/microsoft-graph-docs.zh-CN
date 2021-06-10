---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4f8f5f7fe492d7a91bc5988b9e52c11c2900fb9d
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2021
ms.locfileid: "52869650"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.teams("893075dd-2487-4122-925f-022c42e20265").channels("19:561fbdbbfca848a484f0a6f00ce9dbbd@thread.tacv2")
    .provisionEmail()
    .buildRequest()
    .post();

```