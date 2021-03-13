---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ef10bf664998fbd57f8bec541c9eab562701934e
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50773268"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String string = graphClient.compliance().ediscovery().cases("99e865fc-e29f-479a-ba83-9e58eb017103").operations("63926d4779c243458902328d83f61f53").microsoft.graph.ediscovery.caseExportOperation()
    .getDownloadUrl()
    .buildRequest()
    .get();

```