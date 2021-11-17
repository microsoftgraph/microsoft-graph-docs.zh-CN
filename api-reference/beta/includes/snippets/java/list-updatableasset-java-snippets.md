---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 44ea6898e612cd99bd6813d8eb05c977058cc45c
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "61004295"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UpdatableAssetCollectionPage members = graphClient.admin().windows().updates().updatableAssets("{updatableAssetGroupId}").microsoft.graph.windowsUpdates.updatableAssetGroup().members()
    .buildRequest()
    .get();

```