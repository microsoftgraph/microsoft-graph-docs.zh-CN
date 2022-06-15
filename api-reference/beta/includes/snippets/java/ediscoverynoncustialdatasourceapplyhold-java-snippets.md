---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 696b0bb35e996ca5aaf46e6adac4c9cb91fca6bb
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66092243"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.security().cases().ediscoveryCases("b0073e4e-4184-41c6-9eb7-8c8cc3e2288b").noncustodialDataSources("39333641443238353535383731453339")
    .applyHold()
    .buildRequest()
    .post();

```