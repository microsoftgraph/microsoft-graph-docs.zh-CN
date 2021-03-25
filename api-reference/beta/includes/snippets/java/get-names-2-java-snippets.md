---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4c574b06bb1ea0e7b40f3f1262d312b56993a84d
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51209163"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookNamedItemCollectionPage names = graphClient.me().drive().items("{id}").workbook().names()
    .buildRequest()
    .get();

```