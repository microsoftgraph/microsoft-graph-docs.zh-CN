---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: af982b21ddb6aa2d363eadcf0bd939798102a1f5
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48601634"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SecureScoreControlProfile secureScoreControlProfile = graphClient.security().secureScoreControlProfiles("{id}")
    .buildRequest()
    .get();

```