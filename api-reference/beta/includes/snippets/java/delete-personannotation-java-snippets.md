---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2514322408f85b7f4d8ff73d1e4d0401fe7eada3
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50774227"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.users("{userId}").profile().notes("{id}")
    .buildRequest()
    .delete();

```