---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4ea06121b349759a45dd603e7ccb266b3a881fd6456b20e9492426441e458460
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219562"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IContactFolderDeltaCollectionPage delta = graphClient.me().contactFolders()
    .delta()
    .buildRequest()
    .get();

```