---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f0d2d73f9799212510f8120a0fa21810f79419f9
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50960905"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IPrintJobCollectionPage jobs = graphClient.print().printers("{id}").jobs()
    .buildRequest()
    .get();

```