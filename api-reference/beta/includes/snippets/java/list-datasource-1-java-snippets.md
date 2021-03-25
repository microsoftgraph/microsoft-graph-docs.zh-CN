---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6e507d5b3dbf9d672c2906d023c60b3a34bc76c3
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51209709"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DataSourceCollectionPage additionalSources = graphClient.compliance().ediscovery().cases("{caseId}").sourceCollections("{sourceCollectionId}").additionalSources()
    .buildRequest()
    .get();

```