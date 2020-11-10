---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 27fba2f98ebeff447000f38ac05d4566bdfc167d
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48963810"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IDriveItemDeltaCollectionPage delta = graphClient.me().drive().root()
    .delta("1230919asd190410jlka")
    .buildRequest()
    .get();

```