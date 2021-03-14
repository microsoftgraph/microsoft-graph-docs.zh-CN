---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8cb42fb6c600fd0b83391ed2aff680c6ad7f8f74
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50810535"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var clientContext = "clientContext-value";

var status = RecordingStatus.NotRecording | RecordingStatus.Recording | RecordingStatus.Failed;

await graphClient.Communications.Calls["{call-id}"]
    .UpdateRecordingStatus(status,clientContext)
    .Request()
    .PostAsync();

```