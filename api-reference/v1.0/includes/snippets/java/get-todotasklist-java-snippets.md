---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c07e599e0314151bbe9b31c4f2d043a2edfab5e7
ms.sourcegitcommit: 6ec748ef00d025ee216274a608291be3c1257777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/27/2021
ms.locfileid: "50015652"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ITodoTaskListCollectionPage lists = graphClient.me().todo().lists()
    .buildRequest()
    .get();

```