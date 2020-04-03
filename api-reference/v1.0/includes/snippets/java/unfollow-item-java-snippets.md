---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1e3a1de1b68b19c855829be50a670c2660d004e7
ms.sourcegitcommit: bd40e302ce04b686e86989246ab7c4cc9ad3f320
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/03/2020
ms.locfileid: "43124410"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().drive().items("{item-id}")
    .unfollow()
    .buildRequest()
    .delete();

```