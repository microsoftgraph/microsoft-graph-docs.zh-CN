---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 563b53ef8d6994b156a0698ea5d80f560ef371e4
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51201047"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ColumnDefinitionCollectionPage columns = graphClient.sites("{site-id}").lists("{list-id}").columns()
    .buildRequest()
    .get();

```