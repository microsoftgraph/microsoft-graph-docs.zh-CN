---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ce4cb8a5c210e1ba37e4990499af5d3298fef7b8
ms.sourcegitcommit: 1585d55d3e7030b5fd1f7cfd5de8f9fb8202cd56
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/09/2019
ms.locfileid: "37428849"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().messages("{id}")
    .createReply(null,null)
    .buildRequest()
    .post();

```