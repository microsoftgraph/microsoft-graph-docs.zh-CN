---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0cbb601e1d22705e9e82f4e2cab4d339001022e9
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48970088"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UserPurpose userPurpose = graphClient.customRequest("/me/mailboxSettings/userPurpose", UserPurpose.class)
    .buildRequest()
    .get();

```