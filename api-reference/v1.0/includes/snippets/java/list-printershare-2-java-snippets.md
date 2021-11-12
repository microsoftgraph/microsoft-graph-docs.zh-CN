---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d9643b88b1de806c03aedde5013203b252306720bcc30fd58cb51f5db890b764
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158409"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrinterShareCollectionWithReferencesPage shares = graphClient.print().printers("{printerId}").shares()
    .buildRequest()
    .get();

```