---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a866963aec1d959cb65559a2969c398e2f787d6d5fde4a2a45525a202d255012
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332615"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationClass educationClass = new EducationClass();
educationClass.description = "History - World History 1";
educationClass.displayName = "World History Level 1";

graphClient.education().classes("{class-id}")
    .buildRequest()
    .patch(educationClass);

```