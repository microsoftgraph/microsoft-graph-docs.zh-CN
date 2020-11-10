---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 812e1c46cc5b624a3f77d2c4445be2218e82f2a5
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48978747"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

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
    .query(requestsList)
    .buildRequest()
    .post();

```