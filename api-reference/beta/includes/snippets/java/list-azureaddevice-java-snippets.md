---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6d0697df4778e52b31f2e22024772ea59ddd95dda6f85f5f4faba5c7bf607cae
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333596"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UpdatableAssetCollectionPage updatableAssets = graphClient.admin().windows().updates().updatableAssets()
    .buildRequest()
    .filter("isof('microsoft.graph.windowsUpdates.azureADDevice')")
    .get();

```