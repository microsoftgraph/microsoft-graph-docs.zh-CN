---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4d4796a8c6ff6e73cf8feee8af143025841f18f2
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63338272"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

CustomAccessPackageWorkflowExtension customAccessPackageWorkflowExtension = new CustomAccessPackageWorkflowExtension();
customAccessPackageWorkflowExtension.displayName = "test_action_0124_email";
customAccessPackageWorkflowExtension.description = "this is for graph testing only";

graphClient.identityGovernance().entitlementManagement().accessPackageCatalogs("32efb28c-9a7a-446c-986b-ca6528c6669d").customAccessPackageWorkflowExtensions("98ffaec5-ae8e-4902-a434-5ffc5d3d3cd0")
    .buildRequest()
    .put(customAccessPackageWorkflowExtension);

```