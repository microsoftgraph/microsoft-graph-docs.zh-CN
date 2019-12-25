---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5f46d266a1ec2c48f1098d139a3f4326e903a9dc
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40865816"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Participant participant = graphClient.communications().calls("7531d31f-d10d-44de-802f-c569dbca451c").participants("7e1b4346-85a6-4bdd-abe3-d11c5d420efe")
    .buildRequest()
    .get();

```