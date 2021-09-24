---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9d0111e2500dd3d08abaf08281d4a670bcaaa087
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/24/2021
ms.locfileid: "59507875"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

GroupCollectionWithReferencesPage includedGroups = graphClient.policies().mobileAppManagementPolicies("ab90bacf-55a3-4a3e-839a-aa4b74e4f020").includedGroups()
    .buildRequest()
    .get();

```