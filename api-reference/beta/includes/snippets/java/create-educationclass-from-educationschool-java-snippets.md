---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 02f43786b893334d109876d9a220286e189c4775
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50800116"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.education().schools("10001").classes("11001")
    .buildRequest()
    .delete();

```