---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c93025de88c335cd14746c5459c30eb5ec9f1991c327210211d4f221a4bb329e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104938"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookRange workbookRange = graphClient.me().drive().items("{id}").workbook().tables("{id|name}")
    .dataBodyRange()
    .buildRequest()
    .get();

```