---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 33ffa0ef175f7b08959cd8b85a963ffc38dd2d671335112c81e97dbfb53d86a0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161896"
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