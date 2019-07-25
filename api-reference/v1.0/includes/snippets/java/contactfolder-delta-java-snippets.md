---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 246153d8fa18b4378eed3925d067735fefed80ca
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35883983"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("Prefer", "odata.maxpagesize=2"));

IContactFolderDeltaCollectionPage delta = graphClient.me().contactFolders()
    .delta()
    .buildRequest( requestOptions )
    .get();

```