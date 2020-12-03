---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b3c27a145266a51a2aa68ac45913edf4ccc81586
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/01/2020
ms.locfileid: "49530616"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String callbackUri = "callbackUri-value";

AppHostedMediaConfig mediaConfig = new AppHostedMediaConfig();
mediaConfig.blob = "<Media Session Configuration Blob>";

LinkedList<Modality> acceptedModalitiesList = new LinkedList<Modality>();
acceptedModalitiesList.add(Modality.AUDIO);

graphClient.communications().calls("{id}")
    .answer(callbackUri,mediaConfig,acceptedModalitiesList,null)
    .buildRequest()
    .post();

```