---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f9e6f8bbd509aa5bf26c715b01ca7121b668632b
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50975324"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ProgramControlCollectionPage controls = graphClient.programs("673a7379-9c38-4f01-bd9d-4fda7260b807").controls()
    .buildRequest()
    .get();

```