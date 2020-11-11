---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c5fde4d01e3242d516459a63094072e335ad6f6e
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48983211"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String comment = "comment-value";

Boolean sendResponse = true;

graphClient.me().events("{id}")
    .accept(comment,sendResponse)
    .buildRequest()
    .post();

```