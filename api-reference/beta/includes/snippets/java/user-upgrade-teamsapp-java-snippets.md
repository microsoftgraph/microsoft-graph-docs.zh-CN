---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 98d1975a60511cc13e433d323157a9f8a1b4a131
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48974009"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.users("{id}").teamwork().installedApps("{id}")
    .upgrade()
    .buildRequest()
    .post();

```