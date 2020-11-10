---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5ab438f59ba86b9a8613f7f6a380a9d5e75e575a
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48970002"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ItemEmail itemEmail = graphClient.users("{userId}").profile().emails("{id}")
    .buildRequest()
    .get();

```