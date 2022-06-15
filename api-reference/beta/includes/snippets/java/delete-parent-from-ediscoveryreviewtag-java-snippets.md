---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1f3493666701d29ed8dbdd8050326e71df5ca6a2
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66095362"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.security().cases().ediscoveryCases("58399dff-cebe-478f-b1af-d3227f1fd645").tags("d05c2ef9369d49c293b5a6a6d18a5fd9")
    .buildRequest()
    .delete();

```