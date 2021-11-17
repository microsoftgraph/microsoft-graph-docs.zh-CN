---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9f1e63114fa8500bc8235653c00f547f8e3bf137
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "61021912"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

MobilityManagementPolicy mobilityManagementPolicy = graphClient.policies().mobileDeviceManagementPolicies("ab90bacf-55a3-4a3e-839a-aa4b74e4f020")
    .buildRequest()
    .get();

```