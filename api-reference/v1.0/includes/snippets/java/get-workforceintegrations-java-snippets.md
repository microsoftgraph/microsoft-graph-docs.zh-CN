---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 39452598535b1f6e124bffa3462271a7bb1beec9
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50979353"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkforceIntegrationCollectionPage workforceIntegrations = graphClient.teamwork().workforceIntegrations()
    .buildRequest()
    .get();

```