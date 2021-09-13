---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 920dd3eadb8484cf67a8fab610aaf438ee9f568d677ca55f42344d498f38cae5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104993"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationClass educationClass = new EducationClass();
educationClass.displayName = "String";
educationClass.mailNickname = "String";
educationClass.description = "String";
IdentitySet createdBy = new IdentitySet();
educationClass.createdBy = createdBy;
educationClass.classCode = "String";
educationClass.externalName = "String";
educationClass.externalId = "String";
educationClass.externalSource = EducationExternalSource.SIS;
educationClass.externalSourceDetail = "String";
educationClass.grade = "String";
EducationTerm term = new EducationTerm();
educationClass.term = term;

graphClient.education().classes()
    .buildRequest()
    .post(educationClass);

```