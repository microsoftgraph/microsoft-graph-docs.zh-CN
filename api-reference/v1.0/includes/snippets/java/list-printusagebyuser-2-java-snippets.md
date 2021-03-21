---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 29a84b4f900b7edc3399f73e842574fad9836080
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50959551"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IPrintUsageByUserCollectionPage monthlyPrintUsageByUser = graphClient.reports().monthlyPrintUsageByUser()
    .buildRequest()
    .get();

```