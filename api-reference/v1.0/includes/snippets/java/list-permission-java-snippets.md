---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8d3bf32a951935f1d3cc3ccf569f78f128112f27
ms.sourcegitcommit: ddeee0eec277df06d9e635e5b5c257d14c856273
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/04/2021
ms.locfileid: "60783033"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new QueryOption("search", "{query}"));

SiteCollectionPage sites = graphClient.sites()
    .buildRequest( requestOptions )
    .get();

```