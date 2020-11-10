---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1f5d26cabe8b7f9b19bcdfe887ea8a6047b5083d
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48972256"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ITermCollectionPage children = graphClient.termStore().sets("{setId}").children()
    .buildRequest()
    .get();

```