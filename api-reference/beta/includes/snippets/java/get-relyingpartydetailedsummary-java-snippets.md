---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f9f683c64ed8bebd4b8d56954612a54b36f38585
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48975098"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IReportRootGetRelyingPartyDetailedSummaryCollectionPage getRelyingPartyDetailedSummary = graphClient.reports()
    .getRelyingPartyDetailedSummary("period_value")
    .buildRequest()
    .get();

```