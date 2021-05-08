---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8fd876724f49bbb5a673a82c428c8c6ee6f86791
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52241097"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UpdatableAsset updatableAsset = graphClient.admin().windows().updates().updatableAssets("983f03cd-03cd-983f-cd03-3f98cd033f98")
    .buildRequest()
    .get();

```