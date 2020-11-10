---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a6118bd87382dc1579560e86c1d2157d7aeee603
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48980538"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PersonName personName = graphClient.me().profile().names("{id}")
    .buildRequest()
    .get();

```