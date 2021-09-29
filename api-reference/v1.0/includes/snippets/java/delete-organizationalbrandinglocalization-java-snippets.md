---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 90505ee1be092bb67aa21ed8ccd4b80f8e57c5f2
ms.sourcegitcommit: 36bae3615df41876493b25da478e589d1974f97b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/29/2021
ms.locfileid: "59995806"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.organization("d69179bf-f4a4-41a9-a9de-249c0f2efb1d").branding().localizations("fr-FR")
    .buildRequest()
    .delete();

```