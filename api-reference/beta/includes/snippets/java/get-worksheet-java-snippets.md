---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8535f6ad4ce66beee6164e6686e26676b0cbccfcd2e8058136fc20b20d2d33ec
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903910"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookWorksheet workbookWorksheet = graphClient.me().drive().items("{id}").workbook().worksheets("{id|name}")
    .buildRequest()
    .get();

```