---
description: 自动生成的文件。 不修改
ms.openlocfilehash: b222272e5c82b73283e98623c3450409448e2f36
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35874163"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new QueryOption("$filter", "feature eq 'registration'"));

ICredentialUsageSummaryCollectionPage getCredentialUsageSummary = graphClient.reports()
    .getCredentialUsageSummary('D30')
    .buildRequest( requestOptions )
    .get();

```