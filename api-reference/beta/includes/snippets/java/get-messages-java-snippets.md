---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0cc9f90ef7343117025a98e6b5299e4bb259c789
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48975310"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IMessageCollectionPage messages = graphClient.me().messages()
    .buildRequest()
    .select("sender,subject")
    .get();

```