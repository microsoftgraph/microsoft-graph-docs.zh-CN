---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9ca49a08c06fc71a8d666fcf1b8a8596602fa54f
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66095534"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EdiscoveryCase ediscoveryCase = new EdiscoveryCase();
ediscoveryCase.displayName = "CONTOSO LITIGATION-005";
ediscoveryCase.description = "Project Bazooka";
ediscoveryCase.externalId = "324516";

graphClient.security().cases().ediscoveryCases()
    .buildRequest()
    .post(ediscoveryCase);

```