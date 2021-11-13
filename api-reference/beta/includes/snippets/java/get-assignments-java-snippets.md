---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 32a87d03dca580bda3cb0a3c6ec80286f1478341
ms.sourcegitcommit: c6a8c1cc13ace38d6c4371139ee84707c5c93352
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2021
ms.locfileid: "60890980"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationAssignmentCollectionPage assignments = graphClient.education().classes("{id}").assignments()
    .buildRequest()
    .get();

```