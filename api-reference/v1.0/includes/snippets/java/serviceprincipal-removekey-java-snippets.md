---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b068db05135876bb8b324ed7c69d1abeeab33624
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/04/2020
ms.locfileid: "48905374"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String keyId = "f0b0b335-1d71-4883-8f98-567911bfdca6";

String proof = "eyJ0eXAiOiJ...";

graphClient.servicePrincipals("{id}")
    .removeKey(keyId,proof)
    .buildRequest()
    .post();

```