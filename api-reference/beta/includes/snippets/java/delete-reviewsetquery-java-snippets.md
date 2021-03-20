---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6f5889a0c7be9dd402f103d165af0098f0a5c2f3
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50976059"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.compliance().ediscovery().cases("2eef613a-ca2d-42f4-89fe-84d5198ddedf").reviewSets("b26888b3-e1f5-47c5-bdf2-33d1b90cb2e8").queries("6b5358b0-2ce2-4369-b9cf-65392fe56807")
    .buildRequest()
    .delete();

```