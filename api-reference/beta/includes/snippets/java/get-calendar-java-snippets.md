---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9bd3fa4ae9c7016c48bcee4ebea4823aa444920e
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48960108"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Calendar calendar = graphClient.me().calendar()
    .buildRequest()
    .get();

```