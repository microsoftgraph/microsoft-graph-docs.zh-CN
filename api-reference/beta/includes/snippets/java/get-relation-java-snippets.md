---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3734ff08843d01f5aa610a4390b0028bf4845e3c
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48972242"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IRelationCollectionPage relations = graphClient.termStore().sets("{setId}").relations()
    .buildRequest()
    .get();

```