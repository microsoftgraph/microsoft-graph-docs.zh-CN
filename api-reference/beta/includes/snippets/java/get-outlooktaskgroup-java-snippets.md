---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3a592e8f4a4e38209bc50938844d47ed970033f5
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48978065"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

OutlookTaskGroup outlookTaskGroup = graphClient.me().outlook().taskGroups("AAMkADIyAAAhrbe-AAA=")
    .buildRequest()
    .get();

```