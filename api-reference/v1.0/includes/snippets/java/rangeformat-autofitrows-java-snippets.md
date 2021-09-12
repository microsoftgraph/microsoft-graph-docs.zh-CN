---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f9e8022ddf5be2741ab0e8c7d84a8a003f967d8f8f64a3eed2269e918138d118
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219298"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().drive().items("{id}").workbook().names("{name}")
    .range().format()
    .autofitRows()
    .buildRequest()
    .post();

```