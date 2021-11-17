---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6a48534c6ee7bad5e7fb33fc94a0c658b8892385
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61009811"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.New()
storageLocation := "storageLocation-value"
requestBody.SetStorageLocation(&storageLocation)
options := &msgraphsdk.ExportPersonalDataRequestBuilderPostOptions{
    Body: requestBody,
}
userId := "user-id"
graphClient.UsersById(&userId).ExportPersonalData().Post(options)


```