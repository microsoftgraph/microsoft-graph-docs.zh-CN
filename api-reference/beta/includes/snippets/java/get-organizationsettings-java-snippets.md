---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 37eb0a9edb2326e5311553492d37103bc81da047
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48975483"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Organization organization = graphClient.organization("settings")
    .buildRequest()
    .get();

```