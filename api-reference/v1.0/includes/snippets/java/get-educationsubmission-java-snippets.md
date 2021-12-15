---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ca4e14de41794ec0dd953ce375b59ed4552d824c
ms.sourcegitcommit: c47e3d1f3c5f7e2635b2ad29dfef8fe7c8080bc8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/15/2021
ms.locfileid: "61525982"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationSubmission educationSubmission = graphClient.education().classes("59069eb2-2a09-4d90-bb19-2089cc69d613").assignments("80da1069-a635-4913-813f-d775a5470a8f").submissions("869369de-3e5a-89eb-6f2d-83cd88f860b5")
    .buildRequest()
    .get();

```