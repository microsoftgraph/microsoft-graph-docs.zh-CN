---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4709f81c0d9d1216298d465ff2370876bc9567eb
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50943542"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.education().classes("{class-id}").teachers("{teacher-id}")
    .buildRequest()
    .delete();

```