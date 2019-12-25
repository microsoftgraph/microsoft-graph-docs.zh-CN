---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9b84e4ec0f50727a7ac0e4944604ea49ea19ff77
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40865858"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.communications().calls("2e1a0b00-2db4-4022-9570-243709c565ab")
    .keepAlive()
    .buildRequest()
    .post();

```