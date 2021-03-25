---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ebb6007b7896c9963f8dbae9dfda2c3f1dd7860a
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51210452"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UserSource dataSource = new UserSource();
dataSource.email = "badguy@contoso.com";

graphClient.compliance().ediscovery().cases("{caseId}").sourceCollections("{sourceCollectionId}").additionalSources()
    .buildRequest()
    .post(dataSource);

```