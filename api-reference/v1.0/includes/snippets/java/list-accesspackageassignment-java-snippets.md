---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9ced0eacb1ffc97be497941ccad72d3a4aed490a
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/08/2021
ms.locfileid: "61346614"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessPackageAssignmentCollectionPage assignments = graphClient.identityGovernance().entitlementManagement().assignments()
    .buildRequest()
    .get();

```