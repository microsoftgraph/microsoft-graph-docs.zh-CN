---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f9e66bf40920cfdfd5c39439e92fd8884dff95d4
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/02/2021
ms.locfileid: "51573147"
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