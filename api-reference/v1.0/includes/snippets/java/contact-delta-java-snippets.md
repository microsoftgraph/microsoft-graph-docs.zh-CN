---
description: 自动生成的文件。 不修改
ms.openlocfilehash: f4fb81203d12c4700d3683f68c46684426d7cc6d
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35885159"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("Prefer", "odata.maxpagesize=2"));

IContactDeltaCollectionPage delta = graphClient.me().contactFolders("{id}").contacts()
    .delta()
    .buildRequest( requestOptions )
    .select("displayName")
    .get();

```