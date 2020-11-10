---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9384691df2d12a0539d419ee738e07a430195738
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48966798"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IReportRootGetCredentialUsageSummaryCollectionPage getCredentialUsageSummary = graphClient.reports()
    .getCredentialUsageSummary("D30")
    .buildRequest()
    .filter("feature eq 'registration'")
    .get();

```