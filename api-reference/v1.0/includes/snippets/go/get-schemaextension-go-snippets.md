---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 978c991cb95bcf581c9dfe935f47dcb681323e55
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/08/2022
ms.locfileid: "65946834"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.UserRequestBuilderGetQueryParameters{
    Select: "ext55gb1l09_msLearnCourses",
}
options := &msgraphsdk.UserRequestBuilderGetRequestConfiguration{
    QueryParameters: requestParameters,
}
userId := "user-id"
result, err := graphClient.UsersById(&userId).GetWithRequestConfigurationAndResponseHandler(options, nil)


```