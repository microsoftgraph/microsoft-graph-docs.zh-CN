---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 96d083cb99be4c465d6dfce6727777d0d0125d15
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40871116"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IParticipantCollectionPage participants = graphClient.communications().calls("7531d31f-d10d-44de-802f-c569dbca451c").participants()
    .buildRequest()
    .get();

```