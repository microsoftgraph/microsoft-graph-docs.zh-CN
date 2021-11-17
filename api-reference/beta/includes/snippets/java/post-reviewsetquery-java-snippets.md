---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: baa6ea402e7e0868c79f9796af52c14367962e0da4ae19cabd745bf2b571e50a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161493"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ReviewSetQuery reviewSetQuery = new ReviewSetQuery();
reviewSetQuery.displayName = "My Query 1";
reviewSetQuery.query = "(subject:\"Quarterly Financials\")";

graphClient.compliance().ediscovery().cases("2eef613a-ca2d-42f4-89fe-84d5198ddedf").reviewSets("b26888b3-e1f5-47c5-bdf2-33d1b90cb2e8").queries()
    .buildRequest()
    .post(reviewSetQuery);

```