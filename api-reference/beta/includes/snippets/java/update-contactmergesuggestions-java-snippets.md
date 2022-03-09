---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 067b9f51e5dc18f2dc20da427da381c3f878b32a
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63395130"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ContactMergeSuggestions contactMergeSuggestions = new ContactMergeSuggestions();
contactMergeSuggestions.isEnabled = false;

graphClient.me().settings().contactMergeSuggestions()
    .buildRequest()
    .patch(contactMergeSuggestions);

```