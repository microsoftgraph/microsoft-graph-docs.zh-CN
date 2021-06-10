---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d41dbae54042520cc982fbe646c1b1f39bb7b540
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2021
ms.locfileid: "52869594"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.teams("893075dd-2487-4122-925f-022c42e20265").channels("19:561fbdbbfca848a484f0a6f00ce9dbbd@thread.tacv2")
    .removeEmail()
    .buildRequest()
    .post();

```