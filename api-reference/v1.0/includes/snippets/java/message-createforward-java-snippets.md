---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3bda5f227969c09b0913f165ab43db28acdaf933
ms.sourcegitcommit: 1585d55d3e7030b5fd1f7cfd5de8f9fb8202cd56
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/09/2019
ms.locfileid: "37428789"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().messages("{id}")
    .createForward(null,null,null)
    .buildRequest()
    .post();

```