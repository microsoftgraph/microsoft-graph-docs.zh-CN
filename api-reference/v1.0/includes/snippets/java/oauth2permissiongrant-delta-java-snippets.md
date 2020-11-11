---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cd527f3164b0f5d8eb56e809ca66b652f9d8d6a8
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48983743"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IOAuth2PermissionGrantDeltaCollectionPage delta = graphClient.oauth2PermissionGrants()
    .delta()
    .buildRequest()
    .get();

```