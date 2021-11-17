---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 61a31bcf78789c8d8e16375686bb68b3656fb3a2
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60992766"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

orgContactId := "orgContact-id"
result, err := graphClient.ContactsById(&orgContactId).DirectReports().Get(options)


```