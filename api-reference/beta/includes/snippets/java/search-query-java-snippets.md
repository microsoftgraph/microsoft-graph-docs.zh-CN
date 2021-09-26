---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 33951307511baa343e15a8a0c8bcab12e24bad4a3f2df9cb841b03731b7251a7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218895"
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
        .withQueryAlterationOptions(null)
        .build())
    .buildRequest()
    .post();

```