---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b17de52e2fa67a7bef5fbf0f134a3ecef7001c3b
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50951863"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.education().classes("11014").assignments("19002")
    .buildRequest()
    .delete();

```