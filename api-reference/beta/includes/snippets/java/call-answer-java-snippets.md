---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 42f6a3ba3cf4266eedfcf60a9108fec7490d00b3
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65220300"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String callbackUri = "callbackUri-value";

AppHostedMediaConfig mediaConfig = new AppHostedMediaConfig();
mediaConfig.blob = "<Media Session Configuration Blob>";

LinkedList<Modality> acceptedModalitiesList = new LinkedList<Modality>();
acceptedModalitiesList.add(Modality.AUDIO);

IncomingCallOptions callOptions = new IncomingCallOptions();
callOptions.isContentSharingNotificationEnabled = true;

int participantCapacity = 200;

graphClient.communications().calls("{id}")
    .answer(CallAnswerParameterSet
        .newBuilder()
        .withCallbackUri(callbackUri)
        .withMediaConfig(mediaConfig)
        .withAcceptedModalities(acceptedModalitiesList)
        .withParticipantCapacity(participantCapacity)
        .withCallOptions(callOptions)
        .build())
    .buildRequest()
    .post();

```