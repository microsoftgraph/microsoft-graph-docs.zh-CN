---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 995ca0a41230e8c7a317d6015bdd2f65438e2b35
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61084233"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Security().SecureScoreControlProfiles().Get(options)


```