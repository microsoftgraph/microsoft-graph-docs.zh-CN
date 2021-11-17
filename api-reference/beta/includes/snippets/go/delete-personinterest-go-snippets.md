---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1a165b37340f26c838a26f5bd21d85d26c3cf755
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60997694"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

personInterestId := "personInterest-id"
graphClient.Me().Profile().InterestsById(&personInterestId).Delete(options)


```