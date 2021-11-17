---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ee17ec74195592d45522efa78c6527a4982f2359
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60984898"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

userAccountInformationId := "userAccountInformation-id"
result, err := graphClient.Me().Profile().AccountById(&userAccountInformationId).Get(options)


```