---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b57b98e672ae97142da64bcea95746bbd0bb99f0
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50983278"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ParticipantCollectionPage participants = graphClient.communications().calls("7531d31f-d10d-44de-802f-c569dbca451c").participants()
    .buildRequest()
    .get();

```