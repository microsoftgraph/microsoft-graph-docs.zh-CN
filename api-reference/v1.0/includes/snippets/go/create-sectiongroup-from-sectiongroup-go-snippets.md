---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6a289341c2c48814c66af4d48041d9aca720279a
ms.sourcegitcommit: 6968f5aaf40089684efb0c38a95f6cca353c1d92
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/16/2022
ms.locfileid: "62855758"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetAdditionalData(map[string]interface{}{
    "displayName": "Section group name",
}
options := &msgraphsdk.SectionGroupsRequestBuilderPostOptions{
    Body: requestBody,
}
sectionGroupId := "sectionGroup-id"
graphClient.Me().Onenote().SectionGroupsById(&sectionGroupId).SectionGroups().Post(options)


```