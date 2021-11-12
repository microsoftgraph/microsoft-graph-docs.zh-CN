---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9ead926148741a7e72984dba3fcb7bd2e6551de89b1e21a759909baed7e8c9f2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332405"
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