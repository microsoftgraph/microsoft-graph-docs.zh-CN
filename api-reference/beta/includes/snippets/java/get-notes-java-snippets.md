---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1d088a779337919d5ebb5d41088c49514691c389
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48980733"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IPersonAnnotationCollectionPage notes = graphClient.me().profile().notes()
    .buildRequest()
    .get();

```