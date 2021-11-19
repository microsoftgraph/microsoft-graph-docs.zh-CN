---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 02e8751126b25b89364132dcafe54a423d625780
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61096481"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
storageLocation := "storageLocation-value"
requestBody.SetStorageLocation(&storageLocation)
options := &msgraphsdk.ExportPersonalDataRequestBuilderPostOptions{
    Body: requestBody,
}
userId := "user-id"
graphClient.UsersById(&userId).ExportPersonalData().Post(options)


```