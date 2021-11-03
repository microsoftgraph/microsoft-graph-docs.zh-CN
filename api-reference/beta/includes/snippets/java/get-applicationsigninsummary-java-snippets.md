---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8953c011375297bfcf82c571043dd8c87a3438c8f13ea6a0f782b8a70beb9714
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902938"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ReportRootGetAzureADApplicationSignInSummaryCollectionPage getAzureADApplicationSignInSummary = graphClient.reports()
    .getAzureADApplicationSignInSummary(ReportRootGetAzureADApplicationSignInSummaryParameterSet
        .newBuilder()
        .withPeriod("D7")
        .build())
    .buildRequest()
    .get();

```