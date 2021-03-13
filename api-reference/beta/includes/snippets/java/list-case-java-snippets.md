---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e2353cd3b1b5bb43895970ebd9deb813f8809d60
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50776562"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ICaseCollectionPage cases = graphClient.compliance().ediscovery().cases()
    .buildRequest()
    .get();

```