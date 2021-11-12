---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 10854414da1bba52c40d75919e5880655ca6faa1efd4df4ebd482c688362c0c3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903103"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrintJob printJob = graphClient.print().printers("c05f3726-0d4b-4aa1-8fe9-2eb981bb26fb").jobs("5182")
    .buildRequest()
    .get();

```