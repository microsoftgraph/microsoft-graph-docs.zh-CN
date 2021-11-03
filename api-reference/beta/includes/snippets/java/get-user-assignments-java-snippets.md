---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 938334e292ac0a2dae7a6e49e3a196a2eea8a2a4
ms.sourcegitcommit: 64d27a0e3dcccc9d857e62aace4153e5d98fb3d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60730205"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationAssignmentCollectionPage assignments = graphClient.education().users("80cefd93-8d88-40e2-b5d3-67898383e226").assignments()
    .buildRequest()
    .get();

```