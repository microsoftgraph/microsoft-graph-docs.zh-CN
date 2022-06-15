---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: eb5a41dce65e4b97ecefa61dbd982dea5507bfbf
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66094550"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.policies().authenticationMethodsPolicy().authenticationMethodConfigurations("temporaryAccessPass`")
    .buildRequest()
    .delete();

```