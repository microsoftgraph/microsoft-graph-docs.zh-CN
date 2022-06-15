---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4b862b4cebe7021f26aa11f76823f0bdd54d585f
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66096240"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EdiscoveryCase ediscoveryCase = new EdiscoveryCase();
ediscoveryCase.displayName = "My Case 1 - Renamed";
ediscoveryCase.description = "Updated description";

graphClient.security().cases().ediscoveryCases("22aa2acd-7554-4330-9ba9-ce20014aaae4")
    .buildRequest()
    .patch(ediscoveryCase);

```