---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6bf2198184a6fb679941172743cba53121a7dba3
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61088381"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewPersonName()
nickname := "Kesha"
requestBody.SetNickname(&nickname)
options := &msgraphsdk.PersonNameRequestBuilderPatchOptions{
    Body: requestBody,
}
personNameId := "personName-id"
graphClient.Me().Profile().NamesById(&personNameId).Patch(options)


```