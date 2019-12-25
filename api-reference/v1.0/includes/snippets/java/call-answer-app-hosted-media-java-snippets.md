---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e622ca4706f4e479044063172eebf789a255abdb
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40871137"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String callbackUri = "https://bot.contoso.com/api/calls";

LinkedList<String> acceptedModalitiesList = new LinkedList<String>();
acceptedModalitiesList.add("audio");

AppHostedMediaConfig mediaConfig = new AppHostedMediaConfig();
mediaConfig.blob = "<Media Session Configuration Blob>";

graphClient.communications().calls("57DAB8B1894C409AB240BD8BEAE78896")
    .answer(callbackUri,mediaConfig,acceptedModalitiesList)
    .buildRequest()
    .post();

```