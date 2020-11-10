---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a1149c455a645bdefe3a3d42e7db5e000555ba03
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48981175"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IItemPublicationCollectionPage publications = graphClient.me().profile().publications()
    .buildRequest()
    .get();

```