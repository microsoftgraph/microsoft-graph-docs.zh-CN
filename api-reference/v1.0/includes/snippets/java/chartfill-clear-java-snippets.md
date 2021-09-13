---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ae7e4bdfaff904b5df87408d0cf49854683893d13023b7a31f5152d1853301d9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57378796"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().drive().items("{id}").workbook().worksheets("{id|name}").charts("{name}").format().fill()
    .clear()
    .buildRequest()
    .post();

```