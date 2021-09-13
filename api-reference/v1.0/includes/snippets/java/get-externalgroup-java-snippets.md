---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f3de4b965591ebba68a8ef4116a14e1440b95d3c
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59022483"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ExternalGroup externalGroup = graphClient.external().connections("contosohr").groups("31bea3d537902000")
    .buildRequest()
    .get();

```