---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 382384e6a960535ae022fa89bc6f4fa3fc200f8f
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50967469"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationSchool educationSchool = graphClient.education().schools("10001")
    .buildRequest()
    .get();

```