---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6d9172d6f3db14979a82d04e244eb653f4376a93
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50956247"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IPrinterShareCollectionWithReferencesPage shares = graphClient.print().printers("{printerId}").shares()
    .buildRequest()
    .get();

```