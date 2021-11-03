---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 21d5f956262fd4420fdde7294070dbf1a6d7e8c135290731d64697ea927e80b0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163774"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ColumnDefinitionCollectionPage columns = graphClient.sites("{site-id}").columns()
    .buildRequest()
    .get();

```