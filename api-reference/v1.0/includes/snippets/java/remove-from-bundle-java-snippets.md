---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f65227778bda41a3260c317c1baefaf6f53ffbdb
ms.sourcegitcommit: 0d6d39dd6450e0c5fd6844cb78aead00a0782e46
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2022
ms.locfileid: "63758225"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.drive().bundles("{bundle-id}").children("{item-id}")
    .buildRequest()
    .delete();

```