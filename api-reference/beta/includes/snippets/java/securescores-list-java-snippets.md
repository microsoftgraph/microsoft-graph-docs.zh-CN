---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3ca5be05efd15c02ba6dcad5cfa8603c6ce655a5
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50979789"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SecureScoreCollectionPage secureScores = graphClient.security().secureScores()
    .buildRequest()
    .top(1)
    .get();

```