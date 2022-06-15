---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 50d422bdc7623c86f1ba54d0c7045bc6987bf695
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66095720"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.security().cases().ediscoveryCases("b0073e4e-4184-41c6-9eb7-8c8cc3e2288b").searches("c61a5860-d634-4d14-aea7-d82b6f4eb7af").noncustodialSources("35393639323133394345384344303043").reference()
    .buildRequest()
    .delete();

```