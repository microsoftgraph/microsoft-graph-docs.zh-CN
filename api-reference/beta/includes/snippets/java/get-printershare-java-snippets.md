---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d66f04653edca87252423aba3350fded7be06c05f788e4ae29695efc6ecb26b4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902373"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrinterShare printerShare = graphClient.print().shares("{id}")
    .buildRequest()
    .get();

```