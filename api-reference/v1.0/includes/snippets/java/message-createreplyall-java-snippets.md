---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fee1934a19a947e1ada7d2b936fd8fa47a93465c
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2020
ms.locfileid: "37428850"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().messages("{id}")
    .createReplyAll(null,null)
    .buildRequest()
    .post();

```