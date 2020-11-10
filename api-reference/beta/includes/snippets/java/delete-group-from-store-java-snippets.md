---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3db50375c781c537fe92e9843d71e857f564a15b
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48979921"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.termStore().groups("{groupId}")
    .buildRequest()
    .delete();

```