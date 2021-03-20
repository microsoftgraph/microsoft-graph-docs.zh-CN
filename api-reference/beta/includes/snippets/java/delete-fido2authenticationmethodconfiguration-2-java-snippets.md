---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a4c0c2b5197f7ccf68ef6b7e3e930c00d85d5cf0
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50953996"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.policies().authenticationMethodsPolicy().authenticationMethodConfigurations("TemporaryAccessPass")
    .buildRequest()
    .delete();

```