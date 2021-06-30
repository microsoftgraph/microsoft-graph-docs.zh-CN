---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4edd92584351f5b14578f72bef44770d2211b42d
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53210753"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ServiceHealth serviceHealth = graphClient.admin().serviceAnnouncement().healthOverviews("Microsoft 365 suite")
    .buildRequest()
    .get();

```