---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5d921412bca7ffb4ec3848a2b072284b28d04c88
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61011289"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

personAnnualEventId := "personAnnualEvent-id"
result, err := graphClient.Me().Profile().AnniversariesById(&personAnnualEventId).Get(options)


```