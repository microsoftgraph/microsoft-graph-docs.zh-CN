---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c7a57620bb59c2c02d5b28a21bfc827df3c8c175
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62124199"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String destinationTaskListId = "AAMkAGVjMzJmMWZjLTgyYjgtNGIyNi1hOGQ0LWRjMjNmMGRmOWNiYQAuAAAAAAAboFsPFj7gQqFxG";

graphClient.me().tasks().lists("AAMkAGVjMzJmMWZjLTgyYjgtNGIyNi1hOGQ0LWRjMjNmMGRmOWNiYQAuAAAAAAAboFsPFj7gQpLAt").tasks("AAkALgAAAAAAHYQDEapmEc2byACqAC-EWg0AkOO4xOT")
    .move(BaseTaskMoveParameterSet
        .newBuilder()
        .withDestinationTaskListId(destinationTaskListId)
        .build())
    .buildRequest()
    .post();

```