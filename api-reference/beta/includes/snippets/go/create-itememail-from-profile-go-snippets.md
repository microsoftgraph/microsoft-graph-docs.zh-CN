---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3086e3028445b3f8f01ccacd07b72f08ede560ca
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62132844"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewItemEmail()
address := "Innocenty.Popov@adventureworks.com"
requestBody.SetAddress(&address)
options := &msgraphsdk.EmailsRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Me().Profile().Emails().Post(options)


```