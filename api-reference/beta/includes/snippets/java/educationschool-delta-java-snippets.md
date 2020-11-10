---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d5ea8fd2b828fc671b8d511084db8108fddda041
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48965929"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IEducationSchoolDeltaCollectionPage delta = graphClient.education().schools()
    .delta()
    .buildRequest()
    .get();

```