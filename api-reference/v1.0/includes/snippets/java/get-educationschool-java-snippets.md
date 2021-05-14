---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0afbef9d13a60772e865756b2fd85c9358b3ffb8
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2021
ms.locfileid: "52474884"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationSchool educationSchool = graphClient.education().schools("{educationSchoolId}")
    .buildRequest()
    .get();

```