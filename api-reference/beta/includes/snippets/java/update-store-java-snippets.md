---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 51e1b953030308f17cd9ede2eb9326176188511d
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48972311"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Store store = new Store();
store.defaultLanguageTag = "en-US";

graphClient.termStore()
    .buildRequest()
    .patch(store);

```