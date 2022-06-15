---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d5acab683260983bced426bec8c3d6dc660554df
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66094737"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DataSourceCollectionPage additionalSources = graphClient.security().cases().ediscoveryCases("b0073e4e-4184-41c6-9eb7-8c8cc3e2288b").searches("c61a5860-d634-4d14-aea7-d82b6f4eb7af").additionalSources()
    .buildRequest()
    .get();

```