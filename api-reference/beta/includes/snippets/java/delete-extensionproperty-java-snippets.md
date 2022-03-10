---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9f69010666118934e0e4cc694d31e6aa394f4584
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412373"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.applications("fd918e4b-c821-4efb-b50a-5eddd23afc6f").extensionProperties()
    .buildRequest()
    .delete();

```