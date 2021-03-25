---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 47d5c4ebb5fca9661709732a2e7e1bdf0bf0652a
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51209302"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrinterShareCollectionWithReferencesPage shares = graphClient.print().printers("{printerId}").shares()
    .buildRequest()
    .get();

```