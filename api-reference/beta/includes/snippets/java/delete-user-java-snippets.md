---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: edab56fb2fdfa6d2dd8f671fe866cb6bc412547a
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48976483"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.users("ba9a3254-9f18-4209-aeb3-9e42a35b5be4")
    .buildRequest()
    .delete();

```