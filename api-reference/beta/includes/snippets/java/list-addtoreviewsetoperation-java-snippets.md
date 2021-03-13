---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b289cf339346217056fe0b81b6c347b0d0e443a9
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50772658"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AddToReviewSetOperation addToReviewSetOperation = graphClient.compliance().ediscovery().cases("47746044-fd0b-4a30-acfc-5272b691ba5b").sourceCollections("1a9b4145d8f84e39bc45a7f68c5c5119").addToReviewSetOperation()
    .buildRequest()
    .get();

```