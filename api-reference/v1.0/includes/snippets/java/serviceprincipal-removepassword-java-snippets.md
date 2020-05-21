---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 28c2ff0d0b3cde76cea719991cf56c7492d34190
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/21/2020
ms.locfileid: "44336585"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String keyId = "f0b0b335-1d71-4883-8f98-567911bfdca6";

graphClient.servicePrincipals("{id}")
    .removePassword(keyId)
    .buildRequest()
    .post();

```