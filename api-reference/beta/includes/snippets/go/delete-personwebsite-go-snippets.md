---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c5ad623910c05ebdff90924a9864b2f0ff477438
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411895"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

personWebsiteId := "personWebsite-id"
result, err := graphClient.Me().Profile().WebsitesById(&personWebsiteId).Delete(nil)


```