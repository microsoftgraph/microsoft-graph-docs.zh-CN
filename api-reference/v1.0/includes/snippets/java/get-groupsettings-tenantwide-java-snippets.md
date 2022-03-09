---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2f404690869f532a5e81797d880c8b337be67774
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63393555"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

GroupSetting groupSetting = graphClient.groupSettings("84af2ca5-c274-41bf-86e4-6e374ec4def6")
    .buildRequest()
    .get();

```