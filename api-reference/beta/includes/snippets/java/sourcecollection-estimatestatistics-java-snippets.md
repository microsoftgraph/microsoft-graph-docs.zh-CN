---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 183ff63c0b7a8aaa0ddaf7e47fd010a3e007ea24
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50772721"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.compliance().ediscovery().cases("{caseId}").sourceCollections("{sourceCollectionId}")
    .estimateStatistics()
    .buildRequest()
    .post();

```