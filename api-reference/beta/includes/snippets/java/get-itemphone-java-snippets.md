---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 623e52edfb84730dd532266373a325d646bc9704
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48969931"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IItemPhoneCollectionPage phones = graphClient.me().profile().phones()
    .buildRequest()
    .get();

```