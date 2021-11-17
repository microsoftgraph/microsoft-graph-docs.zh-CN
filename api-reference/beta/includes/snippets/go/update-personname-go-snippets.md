---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e96306dcf12cf2e7190e2af6d12e89d4599b24ae
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60993935"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewPersonName()
nickname := "Kesha"
requestBody.SetNickname(&nickname)
options := &msgraphsdk.PersonNameRequestBuilderPatchOptions{
    Body: requestBody,
}
personNameId := "personName-id"
graphClient.Me().Profile().NamesById(&personNameId).Patch(options)


```