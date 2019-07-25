---
description: 自动生成的文件。 不修改
ms.openlocfilehash: ccd9cb97b3de1378c0aad284da4e72cc141e4b41
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35867550"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IAgreementAcceptanceCollectionPage agreementAcceptances = graphClient.me().agreementAcceptances()
    .buildRequest()
    .get();

```