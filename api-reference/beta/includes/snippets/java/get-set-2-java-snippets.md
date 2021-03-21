---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 81cbde01204a2323b9a6ff34d642473694d16fe1
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50955400"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Set set = graphClient.termStore().sets("{setId}")
    .buildRequest()
    .get();

```