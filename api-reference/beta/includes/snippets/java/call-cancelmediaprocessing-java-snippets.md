---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c40e8916eb51c97ece854872b193adbec5759ec1
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48959821"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String clientContext = "clientContext-value";

graphClient.communications().calls("{id}")
    .cancelMediaProcessing(clientContext)
    .buildRequest()
    .post();

```