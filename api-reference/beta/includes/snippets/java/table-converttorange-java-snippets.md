---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7dbd8fe0c215844d7f27dd497fd7589b85210d1b61392e2be90e3217b779e75b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163630"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().drive().items("{id}").workbook().tables("{id|name}")
    .convertToRange()
    .buildRequest()
    .post();

```