---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 044181959caf0560c80867efb248c214464d7253
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50951633"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.education().classes("{id}").teachers("14012")
    .buildRequest()
    .delete();

```