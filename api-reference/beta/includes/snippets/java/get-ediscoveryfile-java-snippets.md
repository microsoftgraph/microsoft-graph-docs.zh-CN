---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9e1107886fac482113a1b44a90e2e085cf3ef1eb
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66093002"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EdiscoveryFile ediscoveryFile = graphClient.security().cases().ediscoveryCases("58399dff-cebe-478f-b1af-d3227f1fd645").reviewSets("273f11a1-17aa-419c-981d-ff10d33e420f").files("000168cdf05c48d98faac7bff8719726a25da40bb2b9c369fb580b8797abf661")
    .buildRequest()
    .get();

```