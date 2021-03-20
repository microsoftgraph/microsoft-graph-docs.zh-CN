---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6b935ff94910dfa273a6537e92250dd7d167e3f0
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50951469"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IEducationClassCollectionPage classes = graphClient.education().classes()
    .buildRequest()
    .get();

```