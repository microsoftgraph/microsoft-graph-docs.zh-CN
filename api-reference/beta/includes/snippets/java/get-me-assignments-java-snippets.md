---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e146ffe9b57617a960ba504d1fa80ca0e7bea20b
ms.sourcegitcommit: 64d27a0e3dcccc9d857e62aace4153e5d98fb3d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60730226"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationAssignmentCollectionPage assignments = graphClient.education().me().assignments()
    .buildRequest()
    .get();

```