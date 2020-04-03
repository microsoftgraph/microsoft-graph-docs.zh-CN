---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cb1d8e2e71a0aade9a7e2595ac333ffabaed028f
ms.sourcegitcommit: bd40e302ce04b686e86989246ab7c4cc9ad3f320
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/03/2020
ms.locfileid: "43124384"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().drive().items("{item-id}")
    .follow()
    .buildRequest()
    .post();

```