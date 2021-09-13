---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 646746706b1d8661e43b3f330fa9ddb646984b85835c0d4ecce09c62bd8db99f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162575"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ListItem listItem = new ListItem();
FieldValueSet fields = new FieldValueSet();
fields.Title = "Widget";
fields.Color = "Purple";
fields.Weight = 32;
listItem.fields = fields;

graphClient.sites("{site-id}").lists("{list-id}").items()
    .buildRequest()
    .post(listItem);

```