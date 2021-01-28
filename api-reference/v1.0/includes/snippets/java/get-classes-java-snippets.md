---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6b935ff94910dfa273a6537e92250dd7d167e3f0
ms.sourcegitcommit: 6ec748ef00d025ee216274a608291be3c1257777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/27/2021
ms.locfileid: "50015837"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IEducationClassCollectionPage classes = graphClient.education().classes()
    .buildRequest()
    .get();

```