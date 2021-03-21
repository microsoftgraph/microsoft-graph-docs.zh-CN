---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1d1a7d5decae220f706474cd729d0c7754eb22ac
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50971003"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookWorksheet workbookWorksheet = graphClient.me().drive().items("{id}").workbook().worksheets("{id|name}")
    .buildRequest()
    .get();

```