---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: def64b0b3dcf4452b71acebefa383643489308f9
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50980428"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String clientContext = "clientContext-value";

RecordingStatus status = RecordingStatus.NOT_RECORDING;

graphClient.communications().calls("{id}")
    .updateRecordingStatus(CallUpdateRecordingStatusParameterSet
        .newBuilder()
        .withStatus(status)
        .withClientContext(clientContext)
        .build())
    .buildRequest()
    .post();

```