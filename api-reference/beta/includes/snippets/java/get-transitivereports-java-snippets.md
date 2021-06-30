---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f593a26b3bacbcb9824f4e4f14abbfbc6b30f7b7
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53210695"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

int int32 = graphClient.contacts("45b7d2e7-b882-4a80-ba97-10b7a63b8fa4").transitiveReports().count()
    .buildRequest()
    .get();

```