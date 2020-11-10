---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c4eaddb1775fa0aed1992c82a3919bcf2308a298
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48959331"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.teams("{teamId}").channels("{channelId}")
    .completeMigration()
    .buildRequest()
    .post();

```