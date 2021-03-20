---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1f7dcc5f162a48a84c8e2e89a696f59dd123f719
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50953705"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IEducationSchoolCollectionPage schools = graphClient.education().schools()
    .buildRequest()
    .get();

```