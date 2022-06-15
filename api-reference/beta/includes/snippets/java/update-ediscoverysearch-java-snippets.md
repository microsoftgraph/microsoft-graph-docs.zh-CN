---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 37e47636974a06593235f7780256cb544465951b
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66092741"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EdiscoverySearch ediscoverySearch = new EdiscoverySearch();
ediscoverySearch.displayName = "Teams search";

graphClient.security().cases().ediscoveryCases("{ediscoveryCaseId}").searches("{ediscoverySearchId}")
    .buildRequest()
    .patch(ediscoverySearch);

```