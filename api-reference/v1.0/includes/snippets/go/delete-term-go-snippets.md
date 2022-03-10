---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 585e34af5e6db668ac031c7558c6c941b7882427
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412190"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

siteId := "site-id"
setId := "set-id"
termId := "term-id"
result, err := graphClient.SitesById(&siteId).TermStore().SetsById(&setId).TermsById(&termId).Delete(nil)


```