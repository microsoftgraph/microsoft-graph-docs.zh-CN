---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 0cc9f90ef7343117025a98e6b5299e4bb259c789
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35867195"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IMessageCollectionPage messages = graphClient.me().messages()
    .buildRequest()
    .select("sender,subject")
    .get();

```