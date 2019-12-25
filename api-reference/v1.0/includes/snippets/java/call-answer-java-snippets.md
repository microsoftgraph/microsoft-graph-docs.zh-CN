---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 65b1b40ec541c09216ea789d0faaf0461acacd22
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40871129"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String callbackUri = "callbackUri-value";

AppHostedMediaConfig mediaConfig = new AppHostedMediaConfig();
mediaConfig.blob = "<Media Session Configuration Blob>";

LinkedList<String> acceptedModalitiesList = new LinkedList<String>();
acceptedModalitiesList.add("audio");

graphClient.communications().calls("{id}")
    .answer(callbackUri,mediaConfig,acceptedModalitiesList)
    .buildRequest()
    .post();

```