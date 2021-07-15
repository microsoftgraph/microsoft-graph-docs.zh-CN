---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ac11f06fdd7e419165b3f475d8b4302b08ca22f0
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53444134"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.policies().mobileAppManagementPolicies("ab90bacf-55a3-4a3e-839a-aa4b74e4f020").includedGroups("1a9db3ab-0acf-4808-99ae-e8ed581cb2e0").reference()
    .buildRequest()
    .delete();

```