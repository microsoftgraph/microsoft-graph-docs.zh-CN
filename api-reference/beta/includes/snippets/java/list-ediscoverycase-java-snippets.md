---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7e8f00543fd15e8386ceb7b5a29405e2b1ccab21
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66092500"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EdiscoveryCaseCollectionPage ediscoveryCases = graphClient.security().cases().ediscoveryCases()
    .buildRequest()
    .get();

```