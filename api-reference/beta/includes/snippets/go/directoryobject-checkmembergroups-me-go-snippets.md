---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 07a9d966f7b8ecc0851b02866d3a8a6f2a40d22c
ms.sourcegitcommit: e497ed9bb56400bdd2bb53d52ddf057d9966220b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/30/2021
ms.locfileid: "61225011"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetGroupIds( []String {
    "fee2c45b-915a-4a64-b130-f4eb9e75525e",
    "4fe90ae7-065a-478b-9400-e0a0e1cbd540",
}
options := &msgraphsdk.CheckMemberGroupsRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Me().CheckMemberGroups().Post(options)


```