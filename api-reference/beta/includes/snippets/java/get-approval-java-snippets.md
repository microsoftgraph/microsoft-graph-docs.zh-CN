---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: daf214164047eaae5b012067ea01dc6e2fe171b7
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50942601"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Approval approval = graphClient.identityGovernance().entitlementManagement().accessPackageAssignmentApprovals("abd306ef-f7b2-4a10-9fd1-493454322489")
    .buildRequest()
    .get();

```