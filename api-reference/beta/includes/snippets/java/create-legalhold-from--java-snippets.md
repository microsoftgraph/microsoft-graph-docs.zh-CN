---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fc74e8d59cde2aab3b80e2d0f007b9eeadb04b60
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50983892"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

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