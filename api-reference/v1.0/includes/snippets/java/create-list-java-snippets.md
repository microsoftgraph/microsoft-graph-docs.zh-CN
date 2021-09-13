---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0ebaff5c1ce5baad8dc1325360a961ec434e0c30b11968abd19692d5d08d88c3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57409708"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

List list = new List();
list.displayName = "Books";
LinkedList<ColumnDefinition> columnsList = new LinkedList<ColumnDefinition>();
ColumnDefinition columns = new ColumnDefinition();
columns.name = "Author";
TextColumn text = new TextColumn();
columns.text = text;
columnsList.add(columns);
ColumnDefinition columns1 = new ColumnDefinition();
columns1.name = "PageCount";
NumberColumn number = new NumberColumn();
columns1.number = number;
columnsList.add(columns1);
ColumnDefinitionCollectionResponse columnDefinitionCollectionResponse = new ColumnDefinitionCollectionResponse();
columnDefinitionCollectionResponse.value = columnsList;
ColumnDefinitionCollectionPage columnDefinitionCollectionPage = new ColumnDefinitionCollectionPage(columnDefinitionCollectionResponse, null);
list.columns = columnDefinitionCollectionPage;
ListInfo list = new ListInfo();
list.template = "genericList";
list.list = list;

graphClient.sites("{site-id}").lists()
    .buildRequest()
    .post(list);

```