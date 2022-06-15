---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 233f2fd4449c84e1c03f99c58a8551e27191604b
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66094368"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DataSourceCollectionWithReferencesPage custodianSources = graphClient.security().cases().ediscoveryCases("b0073e4e-4184-41c6-9eb7-8c8cc3e2288b").searches("c61a5860-d634-4d14-aea7-d82b6f4eb7af").custodianSources()
    .buildRequest()
    .get();

```