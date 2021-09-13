---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ac29a914820b68215689618c56d578f70bc280de490d0a18b16ab45b989e6196
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162006"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookRange workbookRange = graphClient.me().drive().items("{id}").workbook().names("{name}")
    .range()
    .entireRow()
    .buildRequest()
    .get();

```