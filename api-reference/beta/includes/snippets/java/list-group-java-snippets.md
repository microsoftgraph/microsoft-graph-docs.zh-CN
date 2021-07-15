---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 89ae5aeaf20a3698e6d59d768def626c0b5241ae
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53440960"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

GroupCollectionWithReferencesPage includedGroups = graphClient.policies().mobileDeviceManagementPolicies("ab90bacf-55a3-4a3e-839a-aa4b74e4f020").includedGroups()
    .buildRequest()
    .get();

```