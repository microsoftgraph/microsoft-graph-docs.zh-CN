---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0ab9ef6544f10ada5685244a4cfbe1c4fabd0d360f9eb28511489a71ae95d03b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215931"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookRange workbookRange = graphClient.me().drive().root().workbook().worksheets("{id}")
    .range()
    .rowsAbove()
    .buildRequest()
    .get();

```