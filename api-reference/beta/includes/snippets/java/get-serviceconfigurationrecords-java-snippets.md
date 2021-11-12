---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 31cf3d86bf79912257122ba0038584f43b1ac987fc0a89208b31c7f86657ac63
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218583"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DomainDnsRecordCollectionPage serviceConfigurationRecords = graphClient.domains("contoso.com").serviceConfigurationRecords()
    .buildRequest()
    .get();

```