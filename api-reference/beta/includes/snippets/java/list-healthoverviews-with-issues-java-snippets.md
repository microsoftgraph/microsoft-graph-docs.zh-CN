---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9f32e3d564d795a7bfd579b641f358f56a6c92a4a1e0210f5a8a7674ecd2e823
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106612"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ServiceHealthCollectionPage healthOverviews = graphClient.admin().serviceAnnouncement().healthOverviews()
    .buildRequest()
    .expand("issues")
    .get();

```