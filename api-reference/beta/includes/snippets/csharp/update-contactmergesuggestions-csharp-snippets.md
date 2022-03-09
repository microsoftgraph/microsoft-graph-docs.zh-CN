---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7ac60950a3b1b1f40fb83ec6be610d5f264cdea3
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63395123"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var contactMergeSuggestions = new ContactMergeSuggestions
{
    IsEnabled = false
};

await graphClient.Me.Settings.ContactMergeSuggestions
    .Request()
    .UpdateAsync(contactMergeSuggestions);

```