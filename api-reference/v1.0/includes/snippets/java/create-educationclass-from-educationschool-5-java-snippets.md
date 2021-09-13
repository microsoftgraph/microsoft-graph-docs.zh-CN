---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4f4d1374bf2b1673781cdc4ccdb9ba362c162139db4840df51adfaea9b320ef0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57378256"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationClass educationClass = new EducationClass();
educationClass.additionalDataManager().put("@odata.id", new JsonPrimitive("https://graph.microsoft.com/v1.0/education/classes/11006"));

graphClient.education().schools("{school-id}").classes().references()
    .buildRequest()
    .post(educationClass);

```