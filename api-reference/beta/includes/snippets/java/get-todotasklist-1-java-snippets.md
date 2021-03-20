---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c07e599e0314151bbe9b31c4f2d043a2edfab5e7
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50953811"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ITodoTaskListCollectionPage lists = graphClient.me().todo().lists()
    .buildRequest()
    .get();

```