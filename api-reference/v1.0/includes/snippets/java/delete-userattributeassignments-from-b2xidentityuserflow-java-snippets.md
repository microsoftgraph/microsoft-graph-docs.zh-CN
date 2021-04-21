---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4238b2bf5f5b59f8c4e71700298114d1f2523059
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/21/2021
ms.locfileid: "51920774"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.identity().b2xUserFlows("B2X_1_Partner").userAttributeAssignments("City")
    .buildRequest()
    .delete();

```