---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 525a596e437cc5b03b998211e8d8563a922029bd
ms.sourcegitcommit: df0778a4dbd1e7a2fde1846bdfbfd9440fc91672
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/06/2021
ms.locfileid: "49768196"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new QueryOption("includeHiddenFolders", "true"));

IMailFolderCollectionPage mailFolders = graphClient.me().mailFolders()
    .buildRequest( requestOptions )
    .get();

```