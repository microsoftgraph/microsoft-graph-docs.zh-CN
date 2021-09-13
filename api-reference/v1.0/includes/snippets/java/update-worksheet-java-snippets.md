---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e602a36ae629d18137346782f24477d9b4bcac240aa3389103575e19df5cd093
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333196"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookWorksheet workbookWorksheet = new WorkbookWorksheet();
workbookWorksheet.position = 99;
workbookWorksheet.name = "name-value";
workbookWorksheet.visibility = "visibility-value";

graphClient.me().drive().items("{id}").workbook().worksheets("{id|name}")
    .buildRequest()
    .patch(workbookWorksheet);

```