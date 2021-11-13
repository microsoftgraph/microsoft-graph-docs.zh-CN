---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 446cae947dbce4d30b45fe452f07348946e5fbab
ms.sourcegitcommit: c6a8c1cc13ace38d6c4371139ee84707c5c93352
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2021
ms.locfileid: "60891002"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationAssignmentCollectionPage assignments = graphClient.education().classes("{id}").assignments()
    .buildRequest()
    .expand("resources")
    .get();

```