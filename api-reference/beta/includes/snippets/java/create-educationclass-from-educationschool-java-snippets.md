---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8d174030767cf0e32a6c3e4917c100d06712d584
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48955524"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationClass educationClass = new EducationClass();
educationClass.additionalDataManager().put("@odata.id", new JsonPrimitive("https://graph.microsoft.com/beta/education/classes/11006"));

graphClient.education().schools("10002").classes().references()
    .buildRequest()
    .post(educationClass);

```