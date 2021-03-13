---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ec8ab0619b54362d6a3e9708fcb2019afc652a2e
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50776639"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IReviewSetCollectionPage reviewSets = graphClient.compliance().ediscovery().cases("{caseId}").reviewSets()
    .buildRequest()
    .get();

```