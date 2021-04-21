---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2e7d5280a5d1b7f5c4b375d85babba1e172f7fdf
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/21/2021
ms.locfileid: "51920533"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UserFlowLanguagePageCollectionPage overridesPages = graphClient.identity().b2xUserFlows("B2X_1_Partner").languages("en").overridesPages()
    .buildRequest()
    .get();

```