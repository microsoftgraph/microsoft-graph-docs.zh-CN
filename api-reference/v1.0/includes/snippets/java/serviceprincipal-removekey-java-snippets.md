---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 510b9861cedf224856c13c4476994af0112850d9
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/21/2020
ms.locfileid: "44334881"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String keyId = "f0b0b335-1d71-4883-8f98-567911bfdca6";

String proof = "eyJ0eXAiOiJ...";

graphClient.serviceprincipals("{id}")
    .removeKey(keyId,proof)
    .buildRequest()
    .post();

```