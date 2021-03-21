---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c6849b73e6b585d4e0ac2e5d16c65a47dbf0a48b
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50975926"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DomainDnsRecordCollectionPage serviceConfigurationRecords = graphClient.domains("{domain-name}").serviceConfigurationRecords()
    .buildRequest()
    .get();

```