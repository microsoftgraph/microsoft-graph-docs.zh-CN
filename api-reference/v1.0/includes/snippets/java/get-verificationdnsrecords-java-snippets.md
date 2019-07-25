---
description: 自动生成的文件。 不修改
ms.openlocfilehash: acca8a67beccb78c49c68e6f237306ab50c1898c
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35883134"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IDomainDnsRecordCollectionPage verificationDnsRecords = graphClient.domains("{domain-name}").verificationDnsRecords()
    .buildRequest()
    .get();

```