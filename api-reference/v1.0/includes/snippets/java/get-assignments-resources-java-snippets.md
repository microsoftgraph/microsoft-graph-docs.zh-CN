---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d54c713a1e3f247de203fc56430dbfec22a6cf8a
ms.sourcegitcommit: c6a8c1cc13ace38d6c4371139ee84707c5c93352
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2021
ms.locfileid: "60890720"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationAssignmentCollectionPage assignments = graphClient.education().classes("acdefc6b-2dc6-4e71-b1e9-6d9810ab1793").assignments()
    .buildRequest()
    .expand("resources")
    .get();

```