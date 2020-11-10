---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 41533724b61508cb1a848d4bde4da90bad1fe63f
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48962225"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.applications("{id}").tokenLifetimePolicies("{id}").reference()
    .buildRequest()
    .delete();

```