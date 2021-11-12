---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c65a02707c65f7b1c065373ea692ce246b2864f1f59d2405e61167d572e0e04d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56904002"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookNamedItemCollectionPage names = graphClient.me().drive().items("{id}").workbook().worksheets("{id|name}").names()
    .buildRequest()
    .get();

```