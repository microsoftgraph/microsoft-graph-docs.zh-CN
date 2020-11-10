---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 238b8855b4e415fcc587d864044da9d18c5bda8e
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48979074"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TodoTaskList todoTaskList = graphClient.me().todo().lists("AAMkADIyAAAAABrJAAA=")
    .buildRequest()
    .get();

```