---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ea9bd992cd4b54c1b38b5c9f83bee9d77d6bff49
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48959226"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Channel channel = graphClient.teams("{id}").channels("{id}")
    .buildRequest()
    .get();

```