---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1bc658f2118f7b440855c727551d1f79429e72d5
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48965259"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Group group = graphClient.termStore().groups("{groupId}")
    .buildRequest()
    .get();

```