---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4e7deb7777771bb96794bf191bd27ca561c22aaf
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61018632"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

languageProficiencyId := "languageProficiency-id"
result, err := graphClient.Me().Profile().LanguagesById(&languageProficiencyId).Get(options)


```