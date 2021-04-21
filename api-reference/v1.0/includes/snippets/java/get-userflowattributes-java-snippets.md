---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1097d0efef72d7de94cae6e4c9ee9a81a321152f
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/21/2021
ms.locfileid: "51920914"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IdentityUserFlowAttribute identityUserFlowAttribute = graphClient.identity().userFlowAttributes("{id}")
    .buildRequest()
    .get();

```