---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b0029a720f3291af3811bfce437e39320664bc1e
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50952037"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DataSource dataSource = new DataSource();
dataSource.additionalDataManager().put("@odata.id", new JsonPrimitive("https://graph.microsoft.com/beta/compliance/ediscovery/cases/47746044-fd0b-4a30-acfc-5272b691ba5b/custodians/ab3a628a383045eba344b3caecba3104/userSources/31423539-3846-4333-4136-353644383531"));

graphClient.compliance().ediscovery().cases("47746044-fd0b-4a30-acfc-5272b691ba5b").sourceCollections("1a9b4145d8f84e39bc45a7f68c5c5119").custodianSources().references()
    .buildRequest()
    .post(dataSource);

```