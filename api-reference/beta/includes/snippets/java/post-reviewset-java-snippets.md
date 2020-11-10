---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8f153fa782729f1fecda6d8d4d6015193a47da5e
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48981243"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ReviewSet reviewSet = new ReviewSet();
reviewSet.displayName = "My Reviewset 3";

graphClient.compliance().ediscovery().cases("6f65a8e4-c6a0-4cff-8a81-c9ab5df7290d").reviewSets()
    .buildRequest()
    .post(reviewSet);

```