---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: be15adb230205cca96664080e93438ef28ceff02
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48975915"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.teams("{teamsId}").members("{membership-id}")
    .buildRequest()
    .delete();

```