---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 13b99ca5906deb3b21f83dd9f0c127a599dfe228
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48967894"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String storageLocation = "storageLocation-value";

graphClient.users("{id}")
    .exportPersonalData(storageLocation)
    .buildRequest()
    .post();

```