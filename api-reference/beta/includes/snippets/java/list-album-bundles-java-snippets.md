---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 5b339acd73d3e0531cda2511814896a7e5a965af
ms.sourcegitcommit: 56c0b609dfb1bc5d900956f407d107cdab7086e8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/30/2019
ms.locfileid: "35932641"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new QueryOption("filter", "bundle/album ne null"));
requestOptions.add(new QueryOption("$filter", "bundle/album ne null"));

IDriveItemCollectionPage bundles = graphClient.drive().bundles()
    .buildRequest( requestOptions )
    .get();

```