---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4e2cc2081c77e7d56e48c284a3d69a5c5705d3fb
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65202966"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

List list = graphClient.sites("{siteId}").lists("{listId}")
    .buildRequest()
    .get();

```