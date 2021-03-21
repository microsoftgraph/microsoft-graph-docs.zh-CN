---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8d3bf32a951935f1d3cc3ccf569f78f128112f27
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50976444"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new QueryOption("search", "{query}"));

SiteCollectionPage sites = graphClient.sites()
    .buildRequest( requestOptions )
    .get();

```