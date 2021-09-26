---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d41dbae54042520cc982fbe646c1b1f39bb7b540
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/24/2021
ms.locfileid: "59777156"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.teams("893075dd-2487-4122-925f-022c42e20265").channels("19:561fbdbbfca848a484f0a6f00ce9dbbd@thread.tacv2")
    .removeEmail()
    .buildRequest()
    .post();

```