---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 994d48fbc139a2883336065e82a8d2f4a147cb4d
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50977395"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().drive().root().workbook().worksheets("{id}").pivotTables()
    .refreshAll()
    .buildRequest()
    .post();

```