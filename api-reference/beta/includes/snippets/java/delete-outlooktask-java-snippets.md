---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 07db6d43a7546f0aee476b771be7c0fc80e918ff
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48951516"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().outlook().tasks("AAMkADIyAAAhrb_QAAA=")
    .buildRequest()
    .delete();

```