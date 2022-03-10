---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a39fefec686f049f1da6df5623d7aead8d8e76ae
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412056"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

contactId := "contact-id"
result, err := graphClient.Me().ContactsById(&contactId).Delete(nil)


```