---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 340dd7ecffac9f9dda3773c381185bf39a5b9a21973514b8296b31ba1dc449af
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903487"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookWorksheetCollectionPage worksheets = graphClient.me().drive().items("{id}").workbook().worksheets()
    .buildRequest()
    .get();

```