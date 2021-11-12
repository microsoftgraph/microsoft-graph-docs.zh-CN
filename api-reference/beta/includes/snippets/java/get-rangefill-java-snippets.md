---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 40d7b028a58707aebb8f9ea5c596827b87c7bb85f85fd7e5a95ebbac28409b3f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162758"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookRangeFill workbookRangeFill = graphClient.me().drive().items("{id}").workbook().names("{name}")
    .range().format().fill()
    .buildRequest()
    .get();

```