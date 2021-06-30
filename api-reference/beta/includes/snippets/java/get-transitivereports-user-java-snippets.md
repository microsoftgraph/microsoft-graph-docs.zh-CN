---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 691812f3d2fd99eb8117f57fe974fac704d8482d
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53210825"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

int int32 = graphClient.users("45b7d2e7-b882-4a80-ba97-10b7a63b8fa4").transitiveReports().count()
    .buildRequest()
    .get();

```