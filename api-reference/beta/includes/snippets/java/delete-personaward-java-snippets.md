---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4394323d9d9e735d48055c9b7fea6832ff762845
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50774150"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.users("{userId}").profile().awards("{personAwardId}")
    .buildRequest()
    .delete();

```