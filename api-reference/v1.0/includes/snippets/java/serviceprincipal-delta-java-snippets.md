---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d46cb5b7275538b9783111b2d9235fcabd6778fa
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50972010"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ServicePrincipalDeltaCollectionPage delta = graphClient.servicePrincipals()
    .delta()
    .buildRequest()
    .get();

```