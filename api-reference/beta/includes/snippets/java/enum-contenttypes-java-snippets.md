---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4c3bfaef5c999af6d32e13e515945ff60bded7fc
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50770496"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IContentTypeCollectionPage contentTypes = graphClient.sites("{site-id}").contentTypes()
    .buildRequest()
    .get();

```