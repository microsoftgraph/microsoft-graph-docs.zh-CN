---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ad8c679bf23d67e777f0d413e428078cf316596e
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63394255"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ExtensionProperty extensionProperty = graphClient.applications("fd918e4b-c821-4efb-b50a-5eddd23afc6f").extensionProperties("1f0f15e3-925d-40f0-8fc8-9d3ad135bce0")
    .buildRequest()
    .get();

```