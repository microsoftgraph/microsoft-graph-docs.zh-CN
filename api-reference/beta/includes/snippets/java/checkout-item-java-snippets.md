---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5ba9af93b67c6afab54694e57736753a3f2970c3
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48963842"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.drives("{drive-id}").items("{item-id}")
    .checkout()
    .buildRequest()
    .post();

```