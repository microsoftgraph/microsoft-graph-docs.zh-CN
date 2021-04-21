---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1bda3e69b1c0cb1f1dd34366689307187c67682a
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/21/2021
ms.locfileid: "51920572"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UserFlowLanguageConfiguration userFlowLanguageConfiguration = graphClient.identity().b2xUserFlows("B2X_1_Partner").languages("en")
    .buildRequest()
    .get();

```