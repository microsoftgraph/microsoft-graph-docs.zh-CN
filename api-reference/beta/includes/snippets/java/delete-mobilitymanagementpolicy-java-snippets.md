---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ec1597074a53d5300cf4da35acd7ad4a8c6a56e6
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53440746"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.policies().mobileDeviceManagementPolicies("ab90bacf-55a3-4a3e-839a-aa4b74e4f020")
    .buildRequest()
    .delete();

```