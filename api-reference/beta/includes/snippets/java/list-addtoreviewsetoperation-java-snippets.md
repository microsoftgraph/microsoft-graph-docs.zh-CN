---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3b3b46a242e43d62201a112e2868936aee90eaa3
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50983760"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AddToReviewSetOperation addToReviewSetOperation = graphClient.compliance().ediscovery().cases("47746044-fd0b-4a30-acfc-5272b691ba5b").sourceCollections("1a9b4145d8f84e39bc45a7f68c5c5119").addToReviewSetOperation()
    .buildRequest()
    .get();

```