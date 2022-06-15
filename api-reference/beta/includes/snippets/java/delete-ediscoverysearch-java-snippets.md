---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9ceed4d77cde02ef3411d4d2dc01fb8de85c888e
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66094745"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.security().cases().ediscoveryCases("58399dff-cebe-478f-b1af-d3227f1fd645").searches("60150269-9758-4439-9bc4-453c864d082f")
    .buildRequest()
    .delete();

```