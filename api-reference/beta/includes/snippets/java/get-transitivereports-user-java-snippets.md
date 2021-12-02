---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d72ec8923aee16b2a471c3052253e8bef84844aa452c8be7ec1495fba778c832
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277934"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

int int32 = graphClient.users("45b7d2e7-b882-4a80-ba97-10b7a63b8fa4").transitiveReports().count()
    .buildRequest()
    .get();

```