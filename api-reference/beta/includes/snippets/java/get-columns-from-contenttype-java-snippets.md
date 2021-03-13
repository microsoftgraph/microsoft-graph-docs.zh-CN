---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5ba13e3f7816f7b837d806922aba0b02cc64a701
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50770530"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IColumnDefinitionCollectionPage columns = graphClient.sites("{site-id}").contentTypes("{contentType-id}").columns()
    .buildRequest()
    .get();

```