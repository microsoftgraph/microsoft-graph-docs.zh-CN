---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7c3e8835d2a77439edd8f3374d85717d52cedc42
ms.sourcegitcommit: 3834b7b0287ee71668c52c42d3465ca19366e678
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/01/2020
ms.locfileid: "43082285"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String clientContext = "clientContext-value";

RecordingStatus status = RecordingStatus.NOT_RECORDING;

graphClient.communications().calls("{id}")
    .updateRecordingStatus(status,clientContext)
    .buildRequest()
    .post();

```