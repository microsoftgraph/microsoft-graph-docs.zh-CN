---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 760bfba3717ac205a62de2bcec3f004b7b301ac2
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35888356"
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
list.columns = columnsList;
ListInfo list = new ListInfo();
list.template = "genericList";
list.list = list;

graphClient.sites("{site-id}").lists()
    .buildRequest()
    .post(list);

```