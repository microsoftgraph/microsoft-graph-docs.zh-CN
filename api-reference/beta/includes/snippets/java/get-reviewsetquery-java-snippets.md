---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6ff63635c559a84620fc252936dc34953a719019
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50968229"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ReviewSetQuery reviewSetQuery = graphClient.compliance().ediscovery().cases("2eef613a-ca2d-42f4-89fe-84d5198ddedf").reviewSets("b26888b3-e1f5-47c5-bdf2-33d1b90cb2e8").queries("6b5358b0-2ce2-4369-b9cf-65392fe56807")
    .buildRequest()
    .get();

```