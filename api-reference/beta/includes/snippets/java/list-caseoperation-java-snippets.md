---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: efcd6cf29ee72d3ed8ce54a0d544cf59cfd24d56
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66094172"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

CaseOperationCollectionPage operations = graphClient.security().cases().ediscoveryCases("b0073e4e-4184-41c6-9eb7-8c8cc3e2288b").operations()
    .buildRequest()
    .get();

```