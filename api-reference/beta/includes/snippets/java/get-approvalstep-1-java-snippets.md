---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2d00424a7cb10fe9335503dc22786fb53699db083629131c37ef098c44fcccce
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902930"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ApprovalStepCollectionPage steps = graphClient.identityGovernance().entitlementManagement().accessPackageAssignmentApprovals("abd306ef-f7b2-4a10-9fd1-493454322489").steps()
    .buildRequest()
    .get();

```