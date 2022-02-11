---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4a3be1b6f491501cd706068e93b2e81c1c58c435
ms.sourcegitcommit: 4e16f26b6b685a6a3dae855a04979c84105609b9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/10/2022
ms.locfileid: "62530455"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String callbackUri = "callbackUri-value";

AppHostedMediaConfig mediaConfig = new AppHostedMediaConfig();
mediaConfig.blob = "<Media Session Configuration Blob>";

LinkedList<Modality> acceptedModalitiesList = new LinkedList<Modality>();
acceptedModalitiesList.add(Modality.AUDIO);

int participantCapacity = 200;

graphClient.communications().calls("{id}")
    .answer(CallAnswerParameterSet
        .newBuilder()
        .withCallbackUri(callbackUri)
        .withMediaConfig(mediaConfig)
        .withAcceptedModalities(acceptedModalitiesList)
        .withParticipantCapacity(participantCapacity)
        .withCallOptions(null)
        .build())
    .buildRequest()
    .post();

```