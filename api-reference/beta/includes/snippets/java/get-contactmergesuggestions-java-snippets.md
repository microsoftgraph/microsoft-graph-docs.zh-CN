---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9a349645e94738dc048d7ec493fbbcdc69754eab
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63393947"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ContactMergeSuggestions contactMergeSuggestions = graphClient.me().settings().contactMergeSuggestions()
    .buildRequest()
    .get();

```