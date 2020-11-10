---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8a702590f9170d4184cc7c0014cb1854c62324b4
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48965067"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IEventCollectionPage events = graphClient.groups("{id}").events()
    .buildRequest()
    .get();

```