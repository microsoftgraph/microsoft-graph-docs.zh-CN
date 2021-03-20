---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9b9c19cfa24b4d755c58ce622d95a2ac1a32b9ab
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50974252"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DomainDnsRecordCollectionPage verificationDnsRecords = graphClient.domains("contoso.com").verificationDnsRecords()
    .buildRequest()
    .get();

```