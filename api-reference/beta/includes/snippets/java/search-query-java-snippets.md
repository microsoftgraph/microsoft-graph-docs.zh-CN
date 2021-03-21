---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 65279e1df4abfdc635039fb4c4793459f58fc3c5
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50977718"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<SearchRequest> requestsList = new LinkedList<SearchRequest>();
SearchRequest requests = new SearchRequest();
LinkedList<EntityType> entityTypesList = new LinkedList<EntityType>();
entityTypesList.add(EntityType.EXTERNAL_ITEM);
requests.entityTypes = entityTypesList;
LinkedList<String> contentSourcesList = new LinkedList<String>();
contentSourcesList.add("/external/connections/connectionfriendlyname");
requests.contentSources = contentSourcesList;
SearchQuery query = new SearchQuery();
query.queryString = "contoso product";
requests.query = query;
requests.from = 0;
requests.size = 25;
LinkedList<String> fieldsList = new LinkedList<String>();
fieldsList.add("title");
fieldsList.add("description");
requests.fields = fieldsList;

requestsList.add(requests);

graphClient.search()
    .query(SearchEntityQueryParameterSet
        .newBuilder()
        .withRequests(requestsList)
        .build())
    .buildRequest()
    .post();

```