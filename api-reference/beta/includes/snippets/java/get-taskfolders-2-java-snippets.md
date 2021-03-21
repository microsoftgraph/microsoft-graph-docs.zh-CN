---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0c999e559a954018abc044082ece5908601c0b67
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50957505"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IOutlookTaskFolderCollectionPage taskFolders = graphClient.me().outlook().taskFolders()
    .buildRequest()
    .get();

```