---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c25d52c7488535f0a26daa9b2f921d82ea2c97d0
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50770608"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ContentType contentType = graphClient.sites("{site-id}").contentTypes("{contentType-id}")
    .buildRequest()
    .get();

```