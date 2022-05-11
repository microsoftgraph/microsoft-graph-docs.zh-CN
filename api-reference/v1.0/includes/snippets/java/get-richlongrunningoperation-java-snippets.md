---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b765f69b20f7ffd3df9b9cb1b9571224f61658d0
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65315811"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

RichLongRunningOperation richLongRunningOperation = graphClient.sites("root").operations("contentTypeCopy,0x010100298A15181454D84EBB62EDD7559FCBFE")
    .buildRequest()
    .get();

```