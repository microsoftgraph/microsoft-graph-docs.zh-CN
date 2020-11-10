---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 786c46f077dc94db4c88e153f6db27bf2c90f425
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48953856"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IDirectoryObjectCollectionPage rejectedSenders = graphClient.groups("{id}").rejectedSenders()
    .buildRequest()
    .get();

```