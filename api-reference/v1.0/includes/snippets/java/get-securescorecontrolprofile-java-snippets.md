---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9efe6d13e9eebfab62c2810aa64394a078ecd967
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50976198"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SecureScoreControlProfile secureScoreControlProfile = graphClient.security().secureScoreControlProfiles("{id}")
    .buildRequest()
    .get();

```