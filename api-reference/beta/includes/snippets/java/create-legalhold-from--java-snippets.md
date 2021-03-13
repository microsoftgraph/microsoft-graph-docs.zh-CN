---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e2068de3199b30946472ec75546ed3b7e59259e0
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50773828"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LegalHold legalHold = new LegalHold();
legalHold.description = "String";
IdentitySet createdBy = new IdentitySet();
legalHold.createdBy = createdBy;
legalHold.isEnabled = false;
legalHold.status = LegalHoldStatus.PENDING;
legalHold.contentQuery = "String";
LinkedList<String> errorsList = new LinkedList<String>();
errorsList.add("String");
legalHold.errors = errorsList;
legalHold.displayName = "String";

graphClient.compliance().ediscovery().cases("{caseId}").legalHolds()
    .buildRequest()
    .post(legalHold);

```