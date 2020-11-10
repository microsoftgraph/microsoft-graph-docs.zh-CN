---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7952b4528c31aef6dfd78f5b548642a22b81bcaa
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48965110"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IGroupCollectionPage groups = graphClient.groups()
    .buildRequest()
    .get();

```