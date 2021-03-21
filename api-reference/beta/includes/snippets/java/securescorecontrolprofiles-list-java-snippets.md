---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7131d3578bc52116bfed6133286c7cbecf8b86d2
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50967062"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SecureScoreControlProfileCollectionPage secureScoreControlProfiles = graphClient.security().secureScoreControlProfiles()
    .buildRequest()
    .get();

```