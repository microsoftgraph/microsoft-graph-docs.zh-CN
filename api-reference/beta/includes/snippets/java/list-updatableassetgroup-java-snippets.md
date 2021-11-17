---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f519dbc196e4a410ce72d6411b2e826d2877113702c9e89ad5d207ca0a641a28
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279239"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UpdatableAssetCollectionPage updatableAssets = graphClient.admin().windows().updates().updatableAssets()
    .buildRequest()
    .filter("isof('microsoft.graph.windowsUpdates.updatableAssetGroup')")
    .get();

```