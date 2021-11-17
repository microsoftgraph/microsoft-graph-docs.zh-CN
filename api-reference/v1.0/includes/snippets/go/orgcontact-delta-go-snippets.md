---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 52ad33a2b5e609aa686661d0e0bd0d37e4226d50
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60984503"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

orgContactId := "orgContact-id"
result, err := graphClient.ContactsById(&orgContactId).Get(options)


```