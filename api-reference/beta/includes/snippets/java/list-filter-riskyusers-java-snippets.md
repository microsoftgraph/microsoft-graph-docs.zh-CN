---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 07de26aa6f47224bcf7f5ec618300b11c6d54d66
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50975092"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

RiskyUserCollectionPage riskyUsers = graphClient.identityProtection().riskyUsers()
    .buildRequest()
    .filter("riskLevel eq microsoft.graph.riskLevel'medium'")
    .get();

```