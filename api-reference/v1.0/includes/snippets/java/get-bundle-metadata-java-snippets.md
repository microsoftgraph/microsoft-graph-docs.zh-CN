---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5d1516e9ecd1bbd956fa1700fcdccdb408205442
ms.sourcegitcommit: 0d6d39dd6450e0c5fd6844cb78aead00a0782e46
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2022
ms.locfileid: "63757965"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DriveItem driveItem = graphClient.drive().bundles("{bundle-id}")
    .buildRequest()
    .get();

```