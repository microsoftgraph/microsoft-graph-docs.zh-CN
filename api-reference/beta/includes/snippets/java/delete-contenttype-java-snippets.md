---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4068f957e81f2f8c14d878692ef373e7fb52d4ef
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50770964"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.sites("{site-id}").contentTypes("{contentType-id}")
    .buildRequest()
    .delete();

```