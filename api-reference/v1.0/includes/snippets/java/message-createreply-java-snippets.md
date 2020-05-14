---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ce4cb8a5c210e1ba37e4990499af5d3298fef7b8
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2020
ms.locfileid: "37428849"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().messages("{id}")
    .createReply(null,null)
    .buildRequest()
    .post();

```