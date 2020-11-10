---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 43c3ca6da1b50ddf294d0f7520592f2db1f64f8c
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48976372"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.teams("{id}")
    .archive(null)
    .buildRequest()
    .post();

```