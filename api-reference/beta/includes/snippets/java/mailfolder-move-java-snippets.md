---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 52cfb6b3afe425190e4ddd5e573ea02f84a0edd6
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48979255"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String destinationId = "destinationId-value";

graphClient.me().mailFolders("{id}")
    .move(destinationId)
    .buildRequest()
    .post();

```