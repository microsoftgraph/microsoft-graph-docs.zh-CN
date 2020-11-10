---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9faf3c771188925a914c66a2a198ae1ecf37f0c6
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48979447"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IOutlookTaskCollectionPage tasks = graphClient.me().outlook().tasks()
    .buildRequest()
    .get();

```