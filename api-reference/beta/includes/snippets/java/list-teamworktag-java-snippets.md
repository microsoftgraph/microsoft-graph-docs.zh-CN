---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 06b7236f0ea0fdd914c1e241b8e26a9e9c2670bc
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53210068"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TeamworkTagCollectionPage tags = graphClient.teams("53c53217-fe77-4383-bc5a-ed4937a1aecd").tags()
    .buildRequest()
    .get();

```