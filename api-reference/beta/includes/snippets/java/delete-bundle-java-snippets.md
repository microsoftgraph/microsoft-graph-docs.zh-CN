---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7a7fd056bde8ba2de5f95148c2130000a18be694
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48960270"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.drive().items("{bundle-id}")
    .buildRequest()
    .delete();

```