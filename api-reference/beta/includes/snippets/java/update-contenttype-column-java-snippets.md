---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 36aea46144c3e2049079293e7d79eed8768c4fbd
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50952228"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ColumnDefinition columnDefinition = new ColumnDefinition();
columnDefinition.required = true;
columnDefinition.hidden = false;
columnDefinition.propagateChanges = false;

graphClient.sites("{site-id}").contentTypes("{contentType-id}").columns("{column-id}")
    .buildRequest()
    .patch(columnDefinition);

```