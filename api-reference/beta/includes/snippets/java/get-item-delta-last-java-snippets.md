---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 27fba2f98ebeff447000f38ac05d4566bdfc167d
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36321023"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IDriveItemDeltaCollectionPage delta = graphClient.me().drive().root()
    .delta("1230919asd190410jlka")
    .buildRequest()
    .get();

```