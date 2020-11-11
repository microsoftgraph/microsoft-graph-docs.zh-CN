---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d547204de11f4fed6ed7fe3b697c104d7ac2c412
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48984012"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

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