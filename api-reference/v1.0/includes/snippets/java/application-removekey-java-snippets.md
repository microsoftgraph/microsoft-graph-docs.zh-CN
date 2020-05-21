---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e691d778b0bf4937fe4d66bf08f3a3c3f73ac79b
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/21/2020
ms.locfileid: "44334695"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String keyId = "f0b0b335-1d71-4883-8f98-567911bfdca6";

String proof = "eyJ0eXAiOiJ...";

graphClient.applications("{id}")
    .removeKey(keyId,proof)
    .buildRequest()
    .post();

```