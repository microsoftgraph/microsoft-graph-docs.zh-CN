---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bbfa83466ed98c4830c05c22b88f478166c4b8d7
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66093807"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EdiscoveryReviewSetCollectionPage reviewSets = graphClient.security().cases().ediscoveryCases("b0073e4e-4184-41c6-9eb7-8c8cc3e2288b").reviewSets()
    .buildRequest()
    .get();

```