---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: acd97cf7b8deaaac82b85714c28a45168a9b3388
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52238442"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UpdatableAssetGroup updatableAsset = new UpdatableAssetGroup();

graphClient.admin().windows().updates().updatableAssets()
    .buildRequest()
    .post(updatableAsset);

```