---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f172b073759f738ae40dd47a51e32ba4bfa07633
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50771713"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.print().shares("{printerShareId}").allowedGroups("{groupId}").reference()
    .buildRequest()
    .delete();

```