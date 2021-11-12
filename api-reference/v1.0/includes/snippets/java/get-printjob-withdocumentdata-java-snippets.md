---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a3bc9e9f0e4292b73e9df23a1a8c94780a7e4a5161f7c4d33c42f4f087bacba0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215964"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrintJob printJob = graphClient.print().printers("{printerId}").jobs("{printJobId}")
    .buildRequest()
    .expand("documents")
    .get();

```