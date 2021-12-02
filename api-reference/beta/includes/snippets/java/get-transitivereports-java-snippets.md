---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8edac67e38ef517229b439ac8e5977fb0f8d2de36ba69916b49a8714a89696ef
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332710"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

int int32 = graphClient.contacts("45b7d2e7-b882-4a80-ba97-10b7a63b8fa4").transitiveReports().count()
    .buildRequest()
    .get();

```