---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: db8a745ed4736d9c799e559535dc44c97dcbe7077c5b835c39e2fa766437820c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220721"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookRange workbookRange = graphClient.me().drive().root().workbook().worksheets("{id}")
    .range()
    .rowsBelow()
    .buildRequest()
    .get();

```