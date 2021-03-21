---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d502cb895deb63ff4ee631c65ea82b82c9aaa785
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50981230"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SecureScore secureScore = graphClient.security().secureScores("{id}")
    .buildRequest()
    .get();

```