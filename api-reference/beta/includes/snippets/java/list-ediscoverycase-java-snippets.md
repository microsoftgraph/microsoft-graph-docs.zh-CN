---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e2353cd3b1b5bb43895970ebd9deb813f8809d60
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/16/2020
ms.locfileid: "49692833"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ICaseCollectionPage cases = graphClient.compliance().ediscovery().cases()
    .buildRequest()
    .get();

```