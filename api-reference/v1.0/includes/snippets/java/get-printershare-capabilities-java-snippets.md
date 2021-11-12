---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e3d01e8880b9727ba30665656c8f55f4caff845f2f68f1dc131f640f2209c542
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57378420"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrinterShare printerShare = graphClient.print().shares("{printerShareId}")
    .buildRequest()
    .select("id,displayName,capabilities")
    .get();

```