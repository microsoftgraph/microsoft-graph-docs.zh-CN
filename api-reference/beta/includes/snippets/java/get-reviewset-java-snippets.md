---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2033eee70f254949084cc338cd1530caf68c183d
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48971430"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ReviewSet reviewSet = graphClient.compliance().ediscovery().cases("6f65a8e4-c6a0-4cff-8a81-c9ab5df7290d").reviewSets("0157910c-57ce-4e48-bd4b-90f3c88ca32e")
    .buildRequest()
    .get();

```